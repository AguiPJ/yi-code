<template>
  <h1>
    四象
  </h1>
  <div v-for="(xiang, name) in xiang">
    <h3>{{ name }}</h3>
    <div v-for="yinYang in xiang">
      <Yao :yinYang="yinYang"/>
    </div>
  </div>
</template>

<script>
import Yao from "./Yao.vue";

export default {
  name: "SiXiang",
  components: {Yao},
  setup() {
    const xiang = {
      '少阳': [1, 0],
      '老阳': [1, 1],
      '少阴': [0, 1],
      '老阴': [0, 0]
    }
    return {xiang}
  }
}
</script>

<style scoped>

</style>
