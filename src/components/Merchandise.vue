<template>
  <div id="toggles-box">
    <div class="toggle container d-flex flex-column my-2">
      <i class="fa-solid fa-images"></i> <span>{{ demos }}</span>
    </div>
    <div class="toggle container d-flex flex-column my-2">
      <i class="fa-solid fa-cart-shopping"></i><span>{{ deals }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Merchandise",

  props: {
    demos: String,
    deals: String,
  },
};
</script>

<style scoped lang="scss">
@import "./src/styles/vars.scss";

#toggles-box {
  position: fixed;
  z-index: 2;
  right: 15px;
  top: 15%;
}

span {
  font-weight: bold;
  font-size: 12px;
}

i {
  font-size: 22px;
}

.toggle {
  border: 1px solid black;
  border-radius: 10px;
  display: flex;
  color: #33475b;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  width: 70px;
  height: 70px;
  background-color: white;
  font-family: Arial, Helvetica, sans-serif;
  display: inline-block;

  &:hover {
    color: $ochre;
    cursor: pointer;
  }
}
</style>
