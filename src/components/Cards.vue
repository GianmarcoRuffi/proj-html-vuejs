<template>
  <div class="container"></div>
</template>

<script>
export default {
  name: "Cards",

  props: {
    img: Image,
    title: String,
    text: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

.ochre {
  color: $ochre;
}
</style>
