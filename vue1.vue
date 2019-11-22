<template>
	<div class="row">
		<div id="home" class="col-sm-12 text-center">
			<div class="background">
				<h1>欢迎品尝PIZZA！</h1>
				<h2>这里有很多品种的Pizza！</h2>
				<button @click="gotomenu" class="btn btn-success">Let's go!</button>
			</div>
		</div>
		
	
	
	<h1>Home</h1>
	</div>
</template>

<script>
	export default{
		methods:{
			gotomenu(){
				//跳转到上一个页面
				//this.$router.go(-1)
				
				//指定跳转地址
				//this.$router.replace('/menu')
				
				//指定跳转的路由名字下
				//this.$router.replace({name:'menuLink'})
				
				//通过push进行跳转
				//this.$router.push('/menu')
				this.$router.push({name:'menuLink'})
			}
		}
	}
</script>

<style>
#home{
	background:url('../../src/assets/bg.jpg') ;
	height: 85vh;
	padding: 10%;
}
h1,h2{
	margin:6% ;
}
.background{
	background: #eee;
	opacity: 0.8;/* 透明度 */
	max-width: 70vw;/* vh,vw在谷歌浏览器会有很好的表现*/
	margin: 0 auto;
	padding: 20px 0;
}
</style>
