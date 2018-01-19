<template>
	<div>
		<h2>{{name}}</h2>
		<div @click="change">点击</div>
		<User></User>
	</div>

	
</template>

<script>
	//导入模块

	import User from './components/use.vue'
	export default{
		data:function(){
			return{
				name:"萨达哈市"
			}
		},
		methods:{
			change(){
				this.name = "鼎折覆餗"
			}
		},
		components:{
			User
		}
	}
</script>

<style scoped>
	h2{
		font-size:16px
	}
</style>