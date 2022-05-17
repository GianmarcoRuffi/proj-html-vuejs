<template>
  <div class="container d-flex">
    <div class="component-card col-3">
      <div>
        <img
          src="../assets/img/avadabarbers-homepage-hero-bg.jpg"
          alt=""
          class="img-fluid"
        />
      </div>

      <h1>Prova</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas, quaerat
        illum eius doloribus excepturi repellendus quia maiores sint
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",

  props: {
    img: Image,
    title: String,
    text: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

.component-card {
  text-align: center;

  h1 {
    color: $ochre;
    font-weight: bold;
    padding-top: 5px;
    padding-bottom: 5px;
  }

  p {
    color: #88928f;
    font-family: Arial, Helvetica, sans-serif;
  }
}

.ochre {
  color: $ochre;
}
</style>
