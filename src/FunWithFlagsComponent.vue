<template>
<div>
    <div class="ui fluid search selection dropdown">
        <input type="hidden" name="country">
        <i class="dropdown icon"></i>
        <div class="default text">Select Country</div>
        <div class="menu">
            <div class="item" data-value="af" v-for="f in flags">
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
    name: 'FunWithFlagsCompoenent',
    props: {
        flags: Array
    },
    data () {
        return {
            nationality: ''
        }
    },
    methods: {
        generateFlagClass: function (code) {
			let class_ = code + " flag";
			return class_;
		}
    }
}
</script>

<style scoped>
.menu span {
    text-transform: capitalize;
}
</style>
