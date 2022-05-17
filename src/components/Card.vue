<template>
  <div
    class="component-card col-3 d-flex flex-column justify-content-center align-items-center"
  >
    <img
      :src="require(`../assets/img/${imgURL}`)"
      alt="service"
      class="img-fluid"
    />

    <h1>{{ title }}</h1>
    <p>
      {{ text }}
    </p>
  </div>
</template>

<script>
export default {
  name: "Card",

  props: {
    imgURL: String,
    title: String,
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
  border: 1px solid transparent;

  &:hover {
    cursor: pointer;
    border: 1px solid grey;
    border-radius: 10%;
  }

  h1 {
    color: $ochre;
    font-weight: bold;
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
