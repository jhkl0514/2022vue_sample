<template>
  <HeaderView></HeaderView>
  <main-visual></main-visual>
  <DirectBanner></DirectBanner>
</template>

<script>
 import HeaderView from "./components/HeaderView.vue"
 import MainVisual from "./components/MainVisual.vue";
 import DirectBanner from "./components/DirecBanner.vue"
export default {
  components: {
    HeaderView,
    MainVisual,
    DirectBanner,
}
}
</script>

<style>
*{margin: 0;padding: 0;}
ul,li{list-style: none;}
a:link,a:visited{text-decoration: none;color:#333}
.container{width: 1280px; margin: 0 auto;}
</style>