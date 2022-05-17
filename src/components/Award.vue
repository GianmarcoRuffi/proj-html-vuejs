<template>
  <section id="about">
    <div class="container h-100">
      <div class="row h-100 d-flex justify-content-center align-items-center">
        <div
          class="col-12 col-lg-12 d-flex justify-content-center align-items-center flex-column"
        >
          <h2 class="display-3 py-2 ochre">Award Winning</h2>
          <h1 class="display-5 py-2">Pro barbers</h1>
          <p class="lead">
            <my-button text="Meet your new barber" />
          </p>
        </div>
      </div>
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
export default {
  components: { myButton },
  name: "Award",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#about {
  height: 580px;
  position: relative;
  color: white;
  background-position: top;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-about-introbackground.jpg");
}

.triangle {
  // display: flex;
  // justify-content: center;
  position: absolute;
  bottom: 0;
  width: 100vw;
  // transform: rotate(180deg);
}

ul {
  list-style: none;
  li {
    display: inline-block;
    font-size: 26px;
  }
}

.display-5 {
  font-size: 80px;
}

.hero {
  width: 80%;
}

hr.ochre {
  height: 4px;
  color: $ochre;
}

.ochre {
  color: $ochre;
}

hr {
  font-size: 10px;
  opacity: 1;
}
</style>
