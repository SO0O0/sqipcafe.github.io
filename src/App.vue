<template>
  <CafeHeader />
  <MainVisual />
  <CafeMenu />
</template>

<script>
import CafeHeader from "./components/CafeHeader.vue";
import CafeMenu from "./components/CafeMenu.vue";
import MainVisual from "./components/MainVisual.vue";

export default {
  name: "App",
  components: {
    CafeHeader,
    MainVisual,
    CafeMenu
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
  color: #fff;
  text-decoration: none;
}
</style>
