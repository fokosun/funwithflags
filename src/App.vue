<template>
  <div class="ui grid" id="app">
	  <div class="six wide column">
		  <FunWithFlagsComponent :flags="flags" />
	  </div>
  </div>
</template>

<script>
import FunWithFlagsComponent from './FunWithFlagsComponent.vue'
import flags from './data/all.js'

export default {
	name: 'app',
	computed: {
		flags() {
			let data = Object.values(flags.data)
			return data
		}
	},
	data () {
		return {}
	},
	components: {
		FunWithFlagsComponent
	}
}
</script>
