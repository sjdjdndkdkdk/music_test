<template>
  <router-view/>
  <FooterMusic v-show="$store.state.isFooterMusic"/>
</template>

<script>
// 音乐播放栏在每一个页面都要有，注册全局
import FooterMusic from "./components/item/FooterMusic.vue"
export default {
  components:{
    FooterMusic,
  }
}
</script>

<style lang="less">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.icon {
  width: 0.5rem; 
  height: 0.5rem;
}
</style>
