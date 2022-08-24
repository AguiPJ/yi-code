<script setup>
import Yao from './Yao.vue'

</script>

<template>
  <h1>两仪</h1>
  <div>
    <h3>阳</h3>
    <Yao :yinYang="1"/>
    <h3>阴</h3>
    <Yao :yinYang="0"/>
  </div>
</template>
