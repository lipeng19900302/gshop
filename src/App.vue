<template>
  <div id="app">
    <router-view/>
    <FooterGuide v-show="$route.meta.showFooter" />
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>-->
  </div>
</template>
<script>
import FooterGuide from "./components/FooterGuide/FooterGuide";
export default {
  components: {
    FooterGuide
  }
};
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    width 100%
    height 100%
    background #f5f5f5
</style>
