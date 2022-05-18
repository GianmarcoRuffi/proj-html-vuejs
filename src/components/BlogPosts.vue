<template>
  <section id="blogposts">
    <div class="triangle">
      <svg
        class="fusion-big-triangle-candy"
        xmlns="http://www.w3.org/2000/svg"
        version="1.1"
        width="100%"
        height="100"
        viewBox="0 0 100 100"
        preserveAspectRatio="none"
        style="fill: #ffff; padding: 0"
      >
        <path d="M0 100 L50 2 L100 100 Z"></path>
      </svg>
    </div>
    <div
      class="container h-100 d-flex flex-column justify-content-center align-items-center"
    >
      <div class="row">
        <titles text1="Tales from the barber shop" text2="Recent Blog Posts" />
      </div>
      <div class="row justify-content-center py-4">
        <card-blog
          :imgURL="item.imgURL"
          :name="item.name"
          :text="item.text"
          v-for="(item, index) in blogPosts"
          :key="index"
        />
      </div>
      <div class="row"><my-button text="Read more from our blog" /></div>
    </div>
  </section>
</template>

<script>
import { blogPosts } from "../dati.js";
import myButton from "./myButton.vue";
import Titles from "./Titles.vue";
import CardBlog from "./CardBlog.vue";
export default {
  components: { myButton, Titles, CardBlog },
  name: "BlogPosts",
  data() {
    return {
      blogPosts: blogPosts,
    };
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#blogposts {
  height: 950px;
  position: relative;
  background-color: #f5f5f5;
}

.triangle {
  position: absolute;
  top: 0;
  width: 100%;
  transform: rotate(180deg);
}
</style>
