<template>
	<div>
		<h2>{{name}}</h2>
		<ul>
			<li v-for="use in uses">{{use}}</li>
		</ul>
	</div>
</template>

<script>
	export default{
		data:function(){
			return{
				name:"用户列表",
				uses:['tome','jack','lucy']
			}
		},
		methods:{
			
		}
	}
</script>

<style scoped>
	h2{
		font-size:16px
	}
</style>