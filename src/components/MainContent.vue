<template>
  <section id="about">
    <div class="container h-100">
      <div class="row h-100 d-flex justify-content-center align-items-center">
        <div
          class="col-12 col-lg-12 d-flex justify-content-center align-items-center flex-column"
        >
          <h2 class="display-3 py-2 ochre">Award Winning</h2>
          <h1 class="display-5 py-2">Pro barbers</h1>
          <p class="lead">
            <a class="my-btn" href="#" role="button">Meet your new barber</a>
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default { name: "MainContent" };
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#about {
  height: 480px;
  position: relative;
  color: white;
  background-position: top;
  background-size: cover;
  background-image: url("../assets/img/avadabarbers-about-introbackground.jpg");
}

ul {
  list-style: none;
  li {
    display: inline-block;
    font-size: 26px;
  }
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

.ochre {
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
  width: 300px;
  font-family: Arial, Helvetica, sans-serif;

  &:hover {
    color: white;
    background-color: $ochre;
  }
}
</style>
