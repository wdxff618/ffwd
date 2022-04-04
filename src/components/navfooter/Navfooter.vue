<!-- <template>
	<div>
		<div>
			已完成 {{ isComplete }} / 全部 {{ all }}
			<button type="button" @click="con">清除已完成</button>
		</div>
	</div>
</template>

<script>
	import {defineComponent, ref } from 'vue'
	export default defineComponent ({
		name:'navFooter',
		setup (){
			let isComplete = ref(1)
			let all = ref(3)
			let con = () => {
				console.log('con')
			}
			return{
				isComplete,
				all,
				con
			}
		}
	})
</script>

<style scoped lang="scss">
	
</style>
 -->