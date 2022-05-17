<template>
  <div id="app">
    <Header />
    <Award />
    <services />
    <products />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Award from "./components/Award.vue";
import Services from "./components/Services.vue";
import Products from "./components/Products.vue";

export default {
  name: "App",
  components: { Header, Award, Services, Products },
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
