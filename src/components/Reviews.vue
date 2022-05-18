<template>
  <section id="reviews">
    <div
      class="container h-100 d-flex flex-column justify-content-end align-items-center"
    >
      <div class="featured container">
        <div class="row d-flex">
          <div class="col-4">
            <img
              :src="require(`../assets/img/shaving_butter-800x800.png`)"
              alt="service"
              class="img-fluid"
            />
          </div>
          <div class="col-8">
            <titles
              text1="This months featured product"
              text2="Shaving butter"
            />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Pellentesque laoreet enim est, vel molestie dolor ultrices ut.
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </p>
            <my-button text="Buy now" />
          </div>
        </div>
      </div>

      <div class="row">
        <titles text1="What people say" text2="Reviews" />
      </div>
      <div class="row justify-content-center">
        <card-reviews
          imgURL="avadabarbers-trimcut-gallery6.jpg"
          name="John Doe  "
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis deserunt provident asperiores voluptates repellendus deleniti, ex distinctio autem! Fuga ut totam voluptatibus nihil assumenda quae et atque dolorum labore quasi."
        />
        <card-reviews
          imgURL="avadabarbers-trimcut-gallery7.jpg"
          name="Pete Jones"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis deserunt provident asperiores voluptates repellendus deleniti, ex distinctio autem! Fuga ut totam voluptatibus nihil assumenda quae et atque dolorum labore quasi."
        />
        <card-reviews
          imgURL="avadabarbers-trimcut-gallery3.jpg"
          name="Mark Wilson"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis deserunt provident asperiores voluptates repellendus deleniti, ex distinctio autem! Fuga ut totam voluptatibus nihil assumenda quae et atque dolorum labore quasi."
        />
      </div>
    </div>
  </section>
</template>

<script>
import Titles from "./Titles.vue";
import CardReviews from "./CardReviews.vue";
import myButton from "./myButton.vue";
export default {
  components: { Titles, CardReviews, myButton },
  name: "Services",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#reviews {
  height: 1200px;
  position: relative;
}

.featured {
  background-color: #121413;
  max-height: 40%;
  position: absolute;
  top: -60px;
  max-width: 70%;

  .col-4 {
    background-image: url("../assets/img/avadabarbers-cta-background.jpg");
    background-position: top;
    background-size: cover;
  }
}

.triangle {
  position: absolute;
  bottom: 0;
  width: 100%;
  transform: rotate(180deg);
}
</style>
