<template>
  <div id="app">
   <tab-bar>
   <tab-bar-item path="/home" activeColor='blue'>
   	<img slot="item-icon"  src="./assets/img/tabbar/shouye.png"/>
   	<img slot="item-icon-active" src="./assets/img/tabbar/shouye-activa.png"/>
    <div slot="item-text">首页</div>
   </tab-bar-item>
   
   <tab-bar-item path="/category" activeColor='blue'>
    <img slot="item-icon" src="./assets/img/tabbar/fenlei.png"/>
   	<img slot="item-icon-active" src="./assets/img/tabbar/fenlei-activa.png"/>
    <div slot="item-text">分类</div>
   </tab-bar-item>
   
   <tab-bar-item path="/cart" activeColor='blue'>
   	<img slot="item-icon"  src="./assets/img/tabbar/gwc.png"/>
   	<img slot="item-icon-active" src="./assets/img/tabbar/gwc-activa.png"/>
    <div slot="item-text">购物车</div>
   </tab-bar-item>
   
   <tab-bar-item path="/Profile" activeColor='blue'>
   	<img slot="item-icon"  src="./assets/img/tabbar/wode.png"/>
   	<img slot="item-icon-active"  src="./assets/img/tabbar/wode-activa.png"/>
    <div slot="item-text">我的</div>
   </tab-bar-item>
   
   </tab-bar>
   <router-view></router-view>
  </div>
</template>

<script>
	import TabBar from './components/tabbar/TabBar'
	import TabBarItem from './components/tabbar/TabBarItem'
	
 export default {
  name: 'App',
  components:{
  	TabBar,
  	TabBarItem
  }
}
</script>

<style>
@import "./assets/css/base.css";
</style>
