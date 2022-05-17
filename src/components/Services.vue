<template>
  <section id="services">
    <div class="container h-100">
      <div
        class="row h-100 d-flex justify-content-center align-items-center"
      ></div>
      <my-button />
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
        style="fill: ##121314; padding: 0"
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
  name: "Services",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#services {
  height: 600px;
}
</style>
