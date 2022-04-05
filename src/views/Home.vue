<template>
	<div>
		<NavHeader></NavHeader>
		<NavMain></NavMain>
		<NavFooter></NavFooter>
	</div>
	<!-- <div>
		{{ num }}
	</div>
	<div>
		{{ name }}
	</div> -->
	<!-- <div> -->
		<!-- {{ age.slice(0 , 2) }} vue 插入表达式 -->
		<!-- {{ age }} -->
	<!-- </div> -->
	<!-- <div>
		{{ data.name }} <br>
		{{ data.list }}
	</div>
	<div>
		{{ date.font }}
	</div> -->
	<div>
		{{font+size}}
	</div>
	<div>
		{{ num }}
	</div>
</template>

<script type="text/javascript">
	import NavHeader from '../components/navheader/Navheader.vue'
	import NavMain from '../components/navmain/Navmain.vue'
	import NavFooter from '../components/navfooter/Navfooter.vue'
	import {defineComponent , ref , reactive ,toRefs} from 'vue'
	export default defineComponent({
		name:'Home',
		components:{
			NavHeader,
			NavMain,
			NavFooter
		},
		setup (props, ctx){
			let num = ref(10)
			// let name = ref('可以输入文字吗，哥哥')
			// var age = ref(['1', '2', '3'])
			// let data = ref({
			// 	name:['谢飞宇', '是帅哥', '女朋友也好看'],
			// 	list:['1','2','3']
			// })
			let date = reactive ({
				font:10,
				size: 20,
			})
			return {
				num,
				// name,
				// age,
				// data,
				// date
				...toRefs(date)
			}
		}
	})
</script>

<style scoped lang="scss">
	
</style>
