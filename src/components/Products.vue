<template>
  <section id="products">
    <div
      class="container h-100 d-flex flex-column justify-content-center align-items-center"
    >
      <div class="row">
        <titles text1="We have you covered" text2="Avada Grooming Products" />
      </div>

      <div class="row"><my-button text="Shop our product range" /></div>
    </div>
  </section>
</template>

<script>
import myButton from "./myButton.vue";
import Titles from "./Titles.vue";
export default {
  components: { myButton, Titles },
  name: "Products",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#products {
  height: 920px;
  position: relative;
  color: white;
  background-position: top;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-reviewsbackground.jpg");
}

.container.h-100 {
  padding-bottom: 100px;
}

.ochre {
  color: $ochre;
}
</style>
