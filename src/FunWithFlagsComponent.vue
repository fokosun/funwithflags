<template>
<div>
    <div class="ui fluid search selection dropdown">
        <input type="hidden" name="country">
        <i class="dropdown icon"></i>
        <div class="default text">Select Country</div>
        <div class="menu">
            <div class="item" v-bind:data-value="selectCountryCode(f.code)" v-for="f in flags">
                <i :class="generateFlagClass(f.code)"></i>
                <span class="capitalize">
                    {{ f.country }}
                </span>
                <span class="ui right floated">
                    {{ f.nationality }}
                </span>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import script from './script.js'

export default {
    name: 'FunWithFlagsComponent',
    props: {
        flags: Array
    },
    data () {
        return {
            selectedCountryCode: 'ng'
        }
    },
    methods: {
        generateFlagClass: function (code) {
            let class_ = code + " flag";
            return class_;
        },
        selectCountryCode: function(code) {
            return code
        }
    }
}
</script>

<style scoped>
.menu span {
    text-transform: capitalize;
}
</style>
