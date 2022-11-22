<template>
  <CafeHeader />
  <MainVisual />
  <CafeMenu />
  <CafeNews />
  <CafeAccess />
  <CafeBanner />
  <CafeFooter />
</template>

<script>
import CafeAccess from "./components/CafeAccess.vue";
import CafeBanner from "./components/CafeBanner.vue";
import CafeFooter from "./components/CafeFooter.vue";
import CafeHeader from "./components/CafeHeader.vue";
import CafeMenu from "./components/CafeMenu.vue";
import CafeNews from "./components/CafeNews.vue";
import MainVisual from "./components/MainVisual.vue";

export default {
  name: "App",
  components: {
    CafeHeader,
    MainVisual,
    CafeMenu,
    CafeNews,
    CafeAccess,
    CafeBanner,
    CafeFooter
  }
};
</script>

<style lang="scss">
@charset "UTF-8";

* {
  font-family: Noto Sans CJK JP;
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  vertical-align: baseline;
  background: 0 0;
}

a {
  color : #fff;
  text-decoration: none;
}
</style>

