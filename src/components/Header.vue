<template>
  <section id="jumbotron">
    <div class="container hero h-100 py-4">
      <div class="row h-100">
        <div class="column h-100 d-flex flex-column py-5 justify-content-end">
          <div class="row py-3">
            <div class="col-7 col-md-8 col-lg-3">
              <img
                src="../assets/img/avadabarbers_hero_focalmirror.png"
                alt="barber"
                class="img-fluid"
              />
            </div>
          </div>

          <div class="row">
            <div class="col-12 col-lg-4">
              <h1 class="display-5 py-2">Barber Shop</h1>
              <hr class="ochre" />
              <p class="lead py-2">The pinnacle of male grooming</p>

              <p class="lead">
                <a class="my-btn" href="#" role="button">Learn more</a>
              </p>
            </div>
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
  height: 930px;
  position: relative;
  color: white;
  background-position: center;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-homepage-hero-bg.jpg");
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
