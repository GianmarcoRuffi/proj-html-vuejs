<template>
  <section id="reviews">
    <div
      class="container h-100 d-flex flex-column justify-content-end align-items-center"
    >
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
export default {
  components: { Titles, CardReviews },
  name: "Services",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#reviews {
  height: 1200px;
  position: relative;
}

.triangle {
  position: absolute;
  bottom: 0;
  width: 100%;
  transform: rotate(180deg);
}
</style>
