<template>
  <div id="app">
    <Header />
    <MainContent />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainContent from "./components/MainContent.vue";

export default {
  name: "App",
  components: { Header, MainContent },
};
</script>

<style lang="scss">
@import "./src/styles/general.scss";
#app {
  font-family: "Bodoni Moda", serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
