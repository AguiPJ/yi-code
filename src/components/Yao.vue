<template>
  <div class="yang yao" v-if="yinYang === 1"/>
  <div class="yin yao" v-else />
</template>

<script>
export default {
  name: "Yao",
  props:["yinYang"],
}
</script>

<style scoped>
.yao {
  width: 100px;
  height: 20px;
  background: #000;
  margin: 0 0 15px;
  position: relative;
  display: flex;
  justify-content: center;
}
.yang{
  background: #f00;
}

.yin:before {
  content:'';
  display: inline;
  background: #fff;
  width: 33%;
  height: 110%;
  position: absolute;
  top: -1px;
}
</style>
