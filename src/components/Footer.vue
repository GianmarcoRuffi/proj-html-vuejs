<template>
  <section id="footer">
    <div class="top-footer d-flex justify-content-center align-items-center">
      <div class="container">
        <div class="row d-flex justify-content-center align-items-center">
          <div
            class="component-card col-3 d-flex flex-column justify-content-center align-items-center"
          >
            <img
            :src="require(`../assets/img/avadabarbers_footer_shop_image-300x234.png`)"
            alt="service" class= />

            <my-button text="Shop our range now" />
          </div>
          <div class="middle-row col-3 d-flex align-items-center flex-column">
            <div class="d-block">
              <img
                src="../assets/img/avadabarbers-logo-x1.png"
                alt="barber"
                class="img-fluid"
              />
            </div>

            <ul class="infos">
              <li v-for="(item, index) in footerInfos" :key="index">
                {{ item.text }}
              </li>
            </ul>

            <h5>Follow us</h5>
            <div class="socials">
              <i class="fa-brands fa-facebook-f"></i>
              <i class="fa-brands fa-twitter"></i>
              <i class="fa-brands fa-instagram"></i>
              <i class="fa-brands fa-youtube"></i>
            </div>
          </div>
          <div
            class="component-card col-3 d-flex flex-column justify-content-center align-items-center"
          >
            <img
            :src="require(`../assets/img/avadabarbers_footer_appointment_image-300x234.png`)"
            alt="service" class= />

            <my-button text="Book your appointment" />
          </div>
        </div>
      </div>
    </div>
    <div class="bottom-footer">
      <div class="container d-flex justify-content-center align-items-center">
        <p class="infos">
          &#169; Copyright 2012 - 2022 | Avada Theme by
          <a href="#">ThemeFusion</a> | All Rights Reserved | Powered by
          <a href="#">WordPress</a>
        </p>
      </div>
      <div @click="scrollToTop" id="scroll-toggle">
        <span><i class="fa-solid fa-chevron-up"></i></span>
      </div>
    </div>
  </section>
</template>

<script>
import { footerInfos } from "../dati.js";
import myButton from "./myButton.vue";

export default {
  components: { myButton },
  name: "Footer",

  props: {
    text: String,
  },

  data() {
    return {
      footerInfos: footerInfos,
    };
  },
  methods: {
    scrollToTop() {
      window.scrollTo(0, 0);
    },
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#scroll-toggle {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #5c5c5c;
  color: white;
  width: 50px;
  height: 40px;
  bottom: 0;
  right: 5%;
  border-radius: 5px;

  a {
    color: white;
    text-decoration: none;
  }
  &:hover {
    cursor: pointer;
    background-color: $ochre;
  }
}

#footer {
  height: 700px;
  //   position: relative;

  .top-footer {
    height: 550px;
    background-color: #0f0f0f;

    .socials {
      color: #5c5c5c;
      font-family: Arial, Helvetica, sans-serif;
      text-align: center;
    }

    h5 {
      color: $ochre;
      text-transform: uppercase;
      font-family: Arial, Helvetica, sans-serif;
    }

    ul {
      list-style: none;
      padding-left: 0;
      margin-bottom: 30px;

      li {
        padding-top: 5px;
      }
    }
  }

  .bottom-footer {
    height: 150px;
    background-color: #171717;

    .container {
      height: 100%;
    }

    a {
      text-decoration: none;
      color: $ochre;
    }
  }
}

.infos {
  color: #5c5c5c;
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
}

.socials {
  padding-top: 10px;
  i {
    padding: 10px;
    &:hover {
      cursor: pointer;
      color: $ochre;
    }
  }
}

.component-card {
  text-align: center;

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
</style>
