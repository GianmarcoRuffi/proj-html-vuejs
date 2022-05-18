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

            <p class="infos">
              Avada Barbers <br />
              123 New York Street<br />
              New York City<br />
              info@yourwebsite.com<br />
              +1 (555) 555-1212
            </p>

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
          © Copyright 2012 - 2022 | Avada Theme by <a href="#">ThemeFusion</a> |
          All Rights Reserved | Powered by <a href="#">WordPress</a>
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import myButton from "./myButton.vue";

export default {
  components: { myButton },
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

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
