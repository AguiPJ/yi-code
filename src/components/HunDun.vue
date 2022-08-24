<template>
  <div class="hun-dun">
    <div class="yin">
      <div class="yin-zhong-yang"></div>
    </div>
    <div class="yang">
      <div class="yang-zhong-yin"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HunDun"
}
</script>

<style scoped>
.hun-dun {
  border-radius: 50%;
  background: #787878;
  width: 100px;
  height: 100px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  box-shadow: #787878 0 0 10px;
}


.yin, .yang {
  width: 100px;
  height: 100px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
}

.yin {
  background: #000;
  border-radius: 50px 0 0 50px;
}

.yang {
  background: #fff;
  border-radius: 0 50px 50px 0;
}

.yin-zhong-yang {
  background: #fff;
  transform: translate(25px,25px);
}


.yin-zhong-yang, .yang-zhong-yin {
  width:50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.yang-zhong-yin {
  background: #000;
  transform: translate(-25px,-25px);
}

.yin-zhong-yang::after, .yang-zhong-yin::after{
  content: '';
  display: table;
  background: #000;
  width: 20px;
  height: 20px;
  border-radius: 50%;
}

.yin-zhong-yang::after{
  background: #333;
}
.yang-zhong-yin::after{
  background: #fff;
}
</style>