<template>
  <a class="my-btn" href="#" role="button">{{ text }}</a>
</template>

<script>
export default {
  name: "myButton",

  props: {
    text: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

.my-btn {
  border: 2px solid $ochre;
  display: flex;
  justify-content: center;
  align-items: center;
  color: $ochre;
  text-decoration: none;
  text-transform: uppercase;
  padding: 10px 40px;
  font-family: Arial, Helvetica, sans-serif;
  display: inline-block;
  font-weight: bold;

  &:hover {
    color: white;
    background-color: $ochre;
  }
}
</style>
