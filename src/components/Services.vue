<template>
  <section id="services">
    <div
      class="container h-100 d-flex flex-column justify-content-center align-items-center"
    >
      <div class="row">
        <titles text1="Mens Grooming" text2="Services" />
      </div>
      <div class="row justify-content-center py-4">
        <Card
          imgURL="avadabarbers-trimcut-icon-before.png"
          title="Trim &amp; Cut"
          text="Avada Barbers are experts in the lickety
        split trim and hair cut. Quick but careful and ridicolously good
        looking."
        />
        <Card
          imgURL="avadabarbers-washndry-icon.png"
          title="Wash &amp; Dry"
          text="Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurious fashion."
        />
        <Card
          imgURL="avadabarbers-beardtrim-icon.png"
          title="Beard Tidy"
          text="Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers."
        />
      </div>
      <div class="row"><my-button text="Read about our services" /></div>
    </div>

    <div class="triangle">
      <svg
        class="fusion-big-triangle-candy"
        xmlns="http://www.w3.org/2000/svg"
        version="1.1"
        width="100%"
        height="100"
        viewBox="0 0 100 100"
        preserveAspectRatio="none"
        style="fill: #121314; padding: 0"
      >
        <path d="M0 100 L50 2 L100 100 Z"></path>
      </svg>
    </div>
  </section>
</template>

<script>
import myButton from "./myButton.vue";
import Titles from "./Titles.vue";
import Card from "./Card.vue";
export default {
  components: { myButton, Titles, Card },
  name: "Services",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#services {
  height: 950px;
  position: relative;
}

.triangle {
  position: absolute;
  bottom: 0;
  width: 100%;
  // transform: rotate(180deg);
}
</style>
