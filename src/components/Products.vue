<template>
  <section id="products">
    <div
      class="container h-100 d-flex flex-column justify-content-center align-items-center"
    >
      <div class="row">
        <titles text1="We have you covered" text2="Avada Grooming Products" />
      </div>
      <div class="row justify-content-center py-4">
        <card-products
          imgURL="brush_dark-400x400.png"
          name="Brush"
          price="15.00"
        />
        <card-products
          imgURL="scissors-400x400.png"
          name="Scissors"
          price="85.00"
        />
        <card-products
          imgURL="hot_oil_dark-400x400.png"
          name="Hot Oil"
          price="15.00"
        />
        <card-products
          imgURL="straight_razor_dark-400x400.png"
          name="Straight Razor"
          price="30.00"
        />
      </div>
      <div class="row"><my-button text="Shop our product range" /></div>
    </div>
  </section>
</template>

<script>
import myButton from "./myButton.vue";
import Titles from "./Titles.vue";
import CardProducts from "./CardProducts.vue";
export default {
  components: { myButton, Titles, CardProducts },
  name: "Products",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#products {
  height: 980px;
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
