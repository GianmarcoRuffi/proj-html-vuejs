<template>
  <div class="component-card col-4">
    <div>
      <img :src="require(`../assets/img/${imgURL}`)" alt="" class="img-fluid" />
    </div>

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
