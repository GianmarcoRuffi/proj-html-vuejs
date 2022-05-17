<template>
  <div
    class="component-card col-3 d-flex flex-column justify-content-center align-items-center"
  >
    <p>
      {{ text }}
    </p>

    <img
      :src="require(`../assets/img/${imgURL}`)"
      alt="service"
      class="img-fluid"
    />
    <h5>{{ name }}</h5>
  </div>
</template>

<script>
export default {
  name: "CardReviews",

  props: {
    imgURL: String,
    name: String,
    text: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

img {
  height: 30%;
}

.component-card {
  text-align: center;

  img {
    border-radius: 50%;
    height: 25%;
  }

  h5 {
    color: $ochre;
    font-weight: bold;
    font-style: italic;
    padding-top: 20px;
    padding-bottom: 20px;
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
