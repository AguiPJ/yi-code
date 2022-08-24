<template>
  <div>
    <div v-for="val in yinYangList">
      <Yao :yinYang="val"/>
    </div>
  </div>

</template>

<script>
import Yao from "./Yao.vue";

export default {
  props: ["yinYangList"],
  components: {Yao}
}
</script>
