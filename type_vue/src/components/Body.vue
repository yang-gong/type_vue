<template>
  <div id="body">
   
    <div class="app">
      <select name="xueli" v-model="divclass">
        <option value="red_box">红色</option>
        <option value="green_box">绿色</option>
        <option value="black_box">黑色</option>
      </select>
      <div :class="divclass"></div>

      <input type="radio" value="red_box" name="sex" v-model="divclass" />红色
      <input type="radio" value="green_box" name="sex" v-model="divclass" />绿色
      <input type="radio" value="black_box" name="sex" v-model="divclass" />黑色
    </div>

    <div class="aa"></div>
    <button @click="run()">请点击他</button>
  </div>
</template>

<script>

export default {
  data() {
    return {
      msg:"我是一个身体部位",
      divclass: "",
    };
  },
  methods: {
   run(){
     alert("李小亮孩子你好呀");
   }
  },
 
};
</script>
<style lang="css" scoped>
.red_box {
  height: 100px;
  width: 100px;
  background-color: red;
}

.green_box {
  height: 100px;
  width: 100px;
  background-color: green;
}

.black_box {
  height: 100px;
  width: 100px;
  background-color: black;
}
.aa {
  height: 200px;
  width: 200px;
  background-color: green;
}
h1{
  background-color: red;
}
</style>