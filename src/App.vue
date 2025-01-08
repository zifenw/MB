<template>
  <router-view></router-view>
  <p class="ab">aaaaa</p>
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style lang="less">
// @import url(./styles/commons.less); //以全局引用
@import './assets/fonts/icofont/icofont.css';
.ab{
  font-size: @size-16;
  color: @warning-color;
  background: @gray-2;
}
</style>
