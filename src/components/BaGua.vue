<template>
  <!--  <h1>-->
  <!--    八卦-->
  <!--  </h1>-->
  <div class="box">
    <HunDun class="zhong"/>
    <div v-for="(item, key) in BaGua" :style="`transform:translate(-50%, 0) rotate(${key*45}deg)`" class="Gua-box">
      <h3>
        {{ item.shu }}
      </h3>
      <Gua class="Gua" :yinYangList="item.yao"/>
      <h3>
        {{ item.gua }}
      </h3>
    </div>
  </div>
</template>

<script setup>
import Gua from "./Gua.vue";
import HunDun from "./HunDun.vue";

const BaGua = [
  {
    yao: [1, 1, 1],
    shu: '天',
    gua: '乾'
  },
  {
    yao: [1, 1, 0],
    shu: '风',
    gua: '巽'
  },
  {
    yao: [0, 1, 0],
    shu: '水',
    gua: '坎'
  },
  {
    yao: [1, 0, 0],
    shu: '山',
    gua: '艮'
  },
  {
    yao: [0, 0, 0],
    shu: '地',
    gua: '坤'
  },
  {
    yao: [0, 0, 1],
    shu: '雷',
    gua: '震'
  },
  {
    yao: [1, 0, 1],
    shu: '火',
    gua: '离'
  },
  {
    yao: [0, 1, 1],
    shu: '泽',
    gua: '兑'
  },
]

</script>

<style scoped>
.box {
  position: absolute;
  left: 50vw;
  top: 50vh;
  width: 50vh;
  height: 50vh;
  transform: translate(-50%, -50%);
  /*animation: animal 10s infinite;*/
  animation-timing-function: linear;
  /*background: #3ff;*/
}

.zhong {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}

.Gua-box {
  top: 0;
  left: 50%;
  text-align: center;
  font-size: 11px;
  width: 100px;
  height: 50vh;
  position: absolute;
  /*background: #ddd;*/
  transform: translate(-50%, 0);
}
</style>
