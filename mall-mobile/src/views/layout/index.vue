<template>
  <div class="layout-container">
   <!-- 子路由的出口-->
   <router-view />
   
   <!-- 底部标签导航栏-->
	<van-tabbar route v-model="active">
	  <van-tabbar-item icon="home-o" to="/">首页</van-tabbar-item>
	  <!-- <van-tabbar-item icon="search" to="/category">分类</van-tabbar-item> -->
	  <van-tabbar-item icon="shopping-cart-o" to="/shopCar">购物车</van-tabbar-item>
	  <van-tabbar-item icon="manager-o" to="/my">我的</van-tabbar-item>
	</van-tabbar>
  </div>
</template>

<script>
	export default{
		name:'LayoutIndex',
		data(){
			return {
				 active: 0,
			}
		}
	}
</script>

<style scoped>

</style>