<!-- <template>
	<div v-for="(itme , index) in list" :key="index">
		<div class="itme">
			<input type="checkbox" name="" id="" value="" v-model="itme.complete"/>
			{{ itme.title }}
			<button type="button" @click="del(itme , index)">删除</button>
		</div>
	</div>
</template>

<script>
	import {defineComponent, ref } from 'vue'
	export default defineComponent ({
		name:'navMain',
		setup (){
			let list = ref([
				{title:'吃饭' ,complete: false },
				{title:'睡觉' ,complete: false },
				{title:'敲代码' ,complete: false }
			])
			let del = (itme , index) => {
				console.log(itme)
				console.log(index)
			}
			return{
				list,
				del
			}
		}
	})
</script>

<style scoped lang="scss">
	.itme{
		line-height: 35px;
	}
</style>
 -->