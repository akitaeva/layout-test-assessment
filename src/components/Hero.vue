<template>
  <div class="hero">
    <div class="hero-content">
      <h1 class="heading">Lorem ipsum dolor sit amet</h1>
      <h4>Bibendum est ultricies integer quis.</h4>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Bibendum est
        ultricies integer quis. Iaculis urna id volutpat lacus laoreet. Mauris
        vitae ultricies leo integer malesuada. Ac odio tempor orci dapibus
        ultrices in. Egestas diam in arcu cursus euismod. Dictum fusce ut
      </p>
    </div>
  </div>
</template>

<!-- "scoped" attribute limits CSS to this component only -->
<style scoped lang="less">
.hero {
  width: 100vw;
  height: 100vh;
  min-width: 100%;
  min-height: 100%;
  position: relative;
  text-align: left;
}

&::before {
  background-image: url("./../assets/hero/hero_1.jpg");
  background-size: cover;
  content: "";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -2;
}

.hero-content {
  max-width: 60rem;
  margin: 20rem auto 0;
}

.heading {
  color: #fff;
  font-size: 4rem;
  font-weight: 800;
  letter-spacing: -0.25rem;
}
</style>
