<template>
  <div
    class="component-card col-3 d-flex flex-column justify-content-center align-items-center"
  >
    <img :src="require(`../assets/img/${imgURL}`)" alt="service" class= />

    <h1>{{ name }}</h1>
    <p>&#36;{{ price }}</p>
  </div>
</template>

<script>
export default {
  name: "CardProducts",

  props: {
    imgURL: String,
    name: String,
    price: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

.component-card {
  text-align: center;

  &:hover {
    cursor: pointer;
    background: rgba(128, 128, 128, 0.13);
    border-radius: 10%;
  }

  h1 {
    color: $ochre;
    font-weight: bold;
    padding-top: 20px;
    padding-bottom: 10px;
  }

  p {
    color: $ochre;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px;
  }
}

.ochre {
  color: $ochre;
}
</style>
