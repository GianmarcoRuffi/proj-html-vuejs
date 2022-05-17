<template>
  <div id="app">
    <Header />
    <Award />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Award from "./components/Award.vue";

export default {
  name: "App",
  components: { Header, Award },
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
