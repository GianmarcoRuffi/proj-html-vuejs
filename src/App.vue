<template>
  <div id="app">
    <merchandise demos="Prebuilts" deals="Shopping" />
    <Header />
    <Award />
    <services />
    <products />
    <reviews />
    <blog-posts />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Award from "./components/Award.vue";
import Services from "./components/Services.vue";
import Products from "./components/Products.vue";
import Reviews from "./components/Reviews.vue";
import BlogPosts from "./components/BlogPosts.vue";
import Footer from "./components/Footer.vue";
import Merchandise from "./components/Merchandise.vue";

export default {
  name: "App",
  components: {
    Header,
    Award,
    Services,
    Products,
    Reviews,
    BlogPosts,
    Footer,
    Merchandise,
  },
};
</script>

<style lang="scss">
@import "./src/styles/general.scss";
#app {
  font-family: "Bodoni Moda", serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  position: relative;
}
</style>
