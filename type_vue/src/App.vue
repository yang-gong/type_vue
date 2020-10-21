<template>
  <div id="app">
  <v-home></v-home>   <!-- 使用Home组件-->
  <hr>
   <br>
  <v-body></v-body>
  <br>
  <v-news></v-news>   <!-- 使用News组件-->
 
  </div>
</template>

<script>
/*
1.引入组件

2.挂载组件

3.在模板中使用
*/import Body from './components/Body.vue';
import Home from './components/Home.vue';   //引入首页组件
import News from './components/News.vue';   //引入新闻组件

export default {
  data(){
    return {
      msg:'今天是个好天气'
    }
  },
  components:{  /* 前面的组件名称不能和HTML标签一样*/
    'v-home':Home,    //挂载Home组件  
    'v-news':News,    //挂载新闻组件
    'v-body':Body,     //挂在身体组件
  }
  
}
</script>

<style>

</style>

