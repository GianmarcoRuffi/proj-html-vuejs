<template>
  <section id="jumbotron">
    <div class="container hero h-100 py-4">
      <div class="row d-flex justify-content-between">
        <div class="col-7 col-md-8 col-lg-3">
          <img
            src="../assets/img/avadabarbers-logo-x1.png"
            alt="barber"
            class="img-fluid"
          />
        </div>
        <div class="col-7 col-md-8 col-lg-3 menu">Menu</div>
      </div>
      <!-- *********** -->
      <div
        class="row h-100 py-3 d-flex justify-content-between align-items-center"
      >
        <div class="col-12 col-lg-6">
          <h1 class="display-5 py-2">Barber Shop</h1>
          <hr class="ochre" />
          <p class="lead py-2">The pinnacle of male grooming</p>
          <p class="lead">
            <a class="my-btn" href="#" role="button">Learn more</a>
          </p>
        </div>

        <div class="col-7 col-md-8 col-lg-6 d-flex py-2">
          <div class="col-lg-11">
            <img
              src="../assets/img/avadabarbers_hero_focalmirror.png"
              alt="barber"
              class="img-fluid"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default { name: "Header" };
</script>

<style scoped lang="scss">
@import "../styles/general.scss";
#jumbotron {
  height: 980px;
  position: relative;
  color: white;
  background-position: center;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-homepage-hero-bg.jpg");
}

.display-5 {
  font-size: 80px;
}

.hero {
  width: 80%;
}

hr.ochre {
  height: 4px;
  color: $ochre;
}

hr {
  font-size: 10px;
  opacity: 1;
}

.my-btn {
  border: 2px solid $ochre;
  display: flex;
  justify-content: center;
  align-items: center;
  color: $ochre;
  text-decoration: none;
  text-transform: uppercase;
  padding: 5px;
  width: 200px;

  &:hover {
    color: white;
    background-color: $ochre;
  }
}
</style>
