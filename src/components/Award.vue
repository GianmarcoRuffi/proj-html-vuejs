<template>
  <section id="about">
    <div
      class="container h-100 d-flex flex-column justify-content-center align-items-center"
    >
      <div class="row">
        <titles text1="Award Winning" text2="Pro Barbers" />
      </div>

      <div class="row"><my-button text="Meet your new barber" /></div>
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
        style="fill: #ffff; padding: 0"
      >
        <path d="M0 100 L50 2 L100 100 Z"></path>
      </svg>
    </div>
  </section>
</template>

<script>
import myButton from "./myButton.vue";
import Titles from "./Titles.vue";
export default {
  components: { myButton, Titles },
  name: "Award",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#about {
  height: 520px;

  position: relative;
  color: white;
  background-position: top;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-about-introbackground.jpg");
}

.container.h-100 {
  padding-bottom: 100px;
}

.triangle {
  position: absolute;
  bottom: 0;
  width: 100%;
  // transform: rotate(180deg);
}

.ochre {
  color: $ochre;
}
</style>
