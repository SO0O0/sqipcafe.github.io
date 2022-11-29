<template>
  <CafeHeader />
  <CafeVisual />
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
import CafeVisual from "./components/CafeVisual.vue";

export default {
  name: "App",
  components: {
    CafeHeader,
    CafeVisual,
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
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;300;400;500;700;900&display=swap');

* {
  font-family: 'Noto Sans JP', sans-serif;
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  vertical-align: baseline;
  background: 0 0;
}

a {
  color: #fff;
  text-decoration: none;
}
</style>

