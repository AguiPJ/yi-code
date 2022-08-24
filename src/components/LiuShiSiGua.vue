<template>
  <h1>六十四卦</h1>
  <div v-for="(sgua, shangGua) in BaGua" >

    <div v-for="(xgua, xiaGua) in BaGua" >
      <h3>
        {{shangGua}} + {{xiaGua}}
      </h3>
      <Gua :yinYangList="sgua" />
      <Gua :yinYangList="xgua" />
    </div>
  </div>
</template>

<script>
import Yao from "./Yao.vue";
import Gua from "./Gua.vue";

export default {
  name: "LiuShiSiGua",
  components:{Gua, Yao},
  setup(){
    const BaGua = {
      乾:[1,1,1],//天
      巽:[1,1,0],//风
      离:[1,0,1],//火
      兑:[0,1,1],//泽
      艮:[1,0,0],//山
      坎:[0,1,0],//水
      震:[0,0,1],//雷
      坤:[0,0,0],//地
    }
    return {BaGua}
  }
}
</script>

<style scoped>

</style>
