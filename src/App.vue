<script setup>
import LiangYi from './components/LiangYi.vue' //两仪
import SiXiang from './components/SiXiang.vue'
import BaGua from './components/BaGua.vue'
import LiuShiSiGua from "./components/LiuShiSiGua.vue";
</script>

<template>
  <div class="container">
    <BaGua/>
  </div>
<!--<div class="zhou-xian">-->
<!--  <div class="x"></div>-->
<!--  <div class="y"></div>-->
<!--</div>-->
<!--  <div class="container">-->
<!--    <LiangYi/>-->
<!--    <div class="blank"/>-->
<!--    <SiXiang/>-->
<!--    <div class="blank"/>-->
<!--  </div>-->
<!--  <div class="container">-->
<!--    <liu-shi-si-gua/>-->
<!--  </div>-->
</template>

<style scoped >

.container {
  display: flex;
  justify-content: center;
}

.x{
  position: fixed;
  top: 50vh;
  width: 100vw;
  height: 1px;
  background: #000;
}


.y{
  position: fixed;
  left: 50vw;
  width: 1px;
  height: 100vh;
  background: #000;
}

</style>
