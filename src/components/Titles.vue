<template>
  <div class="container">
    <div class="row d-flex justify-content-center align-items-center">
      <div class="col-12 d-flex justify-content-center align-items-center">
        <h2 class="display-3 ochre">{{ text1 }}</h2>
      </div>
      <div class="col-12 d-flex justify-content-center align-items-center">
        <h1 class="display-5">{{ text2 }}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Titles",

  props: {
    text1: String,
    text2: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

.display-5 {
  font-size: 70px;
  font-weight: bolder;
  color: #b1b1b1;
}

.display-3 {
  text-transform: uppercase;
  font-weight: bold;
  font-size: 18px;
  font-family: Arial, Helvetica, sans-serif;
}

.ochre {
  color: $ochre;
}
</style>
