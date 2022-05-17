<template>
  <div id="app">
    <Header />
    <Award />
    <services />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Award from "./components/Award.vue";
import Services from "./components/Services.vue";

export default {
  name: "App",
  components: { Header, Award, Services },
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
