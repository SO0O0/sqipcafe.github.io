<template>
  <CafeHeader />
  <MainVisual />
</template>

<script>
import CafeHeader from "./components/CafeHeader.vue";
import MainVisual from "./components/MainVisual.vue";

export default {
  name: "App",
  components: {
    CafeHeader,
    MainVisual
  }
};
</script>

<style lang="scss">
@charset "UTF-8";

* {
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  vertical-align: baseline;
  background: 0 0;
}
</style>
