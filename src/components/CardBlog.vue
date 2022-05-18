<template>
  <div
    class="component-card col-4 d-flex flex-column justify-content-center align-items-center"
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

.component-card {
  text-align: center;

  &:hover {
    cursor: pointer;
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
