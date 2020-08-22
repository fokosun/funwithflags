<template>
<div class="ui grid">
    <div class="three wide column">
        {{ nationality }}
     </div>
     <div class="three wide column">
        <select class="ui dropdown">
            <option value="1" v-for="flagObject in flags">
                {{ flagObject.code }}
            </option>
        </select>
     </div>
     <div class="three wide column">
         <i class=""></i>
    </div>
</div>
</template>

<script>
export default {
    name: 'FunWithFlagsCompoenent',
    props: {
        flags: Array
    },
    data () {
        return {
            nationality: '',
            _class: ''
        }
    }
}
</script>
