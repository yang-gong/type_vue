<template>
  <div>
    <div class="div1">
      <h1 class="h1">我是头部组件 -----{{ msg }}</h1>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      msg: "有可能是淘宝首页",
    };
  },
};
</script>
<style scoped>
.h1 {
  position: initial;
  text-align: center;
  color: aqua;
}

.div1 {
  height: 200px;
  width: 100%;
  background-color: #f5f5f5;
  border: 1px solid black;
}
</style>

