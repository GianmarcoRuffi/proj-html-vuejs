<template>
  <section id="reviews">
    <div
      class="container h-100 d-flex flex-column justify-content-end align-items-center"
    >
      <div class="featured container">
        <div class="row d-flex">
          <div
            class="col-4 butter-spot d-flex justify-content-center align-items-center"
          >
            <img
              :src="require(`../assets/img/shaving_butter-800x800.png`)"
              alt="service"
              class="img-fluid"
            />
          </div>
          <div
            class="col-8 d-flex justify-content-center flex-column align-items-left"
          >
            <div class="row d-flex align-items-center">
              <div class="col-12 d-flex align-items-center">
                <h2 class="display-3 ochre">This months featured product</h2>
              </div>
              <div class="col-12 d-flex align-items-center">
                <h1 class="display-5">Shaving Butter</h1>
              </div>
            </div>

            <div>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Pellentesque laoreet enim est, vel molestie dolor ultrices ut.
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              </p>
            </div>
            <div><my-button text="Buy now" /></div>
          </div>
        </div>
      </div>

      <div class="row">
        <titles text1="What people say" text2="Reviews" />
      </div>
      <div class="row justify-content-center py-3">
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
  background-color: #000000;
  max-height: 70%;
  position: absolute;
  top: -60px;
  max-width: 60%;
  border-top: 4px solid $ochre;
  .display-5 {
    font-size: 70px;
    font-weight: bolder;
    color: #b1b1b1;
  }

  .display-3 {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 18px;
    font-family: Arial, Helvetica, sans-serif;
  }

  .ochre {
    color: $ochre;
  }

  p {
    color: #5c5c5c;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 18px;
  }

  .butter-spot {
    background-image: url("../assets/img/avadabarbers-cta-background.jpg");
    background-position: top;
    background-size: cover;
    height: 450px;
  }

  .col-8 {
    padding-left: 8%;
    padding-right: 8%;
  }
}

.triangle {
  position: absolute;
  bottom: 0;
  width: 100%;
  transform: rotate(180deg);
}
</style>
