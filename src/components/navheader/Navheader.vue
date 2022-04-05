<template>
	<div>
		<input type="text" placeholder="请输入任务" v-model="value" @keydown.enter="enter"/>
	</div>
</template>

<script>
	import {defineComponent, ref} from 'vue'
	export default defineComponent ({
		name:'navHeader',
		setup (){
			let vlaue = ref('')
			
			// 按回车确认
			let enter = () =>{
				console.log(vlaue.value)
			}
			return {
				vlaue,
				enter
			}
		},
	})
</script>

<style scoped lang="scss">
	
</style>
