<template>
  <div class="hero">
    <div class="hero-content">
      <h1 class="heading">Lorem ipsum dolor sit amet</h1>
      <h4 class="subheading">Bibendum est ultricies integer quis.</h4>
      <p class="hero-text">
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
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: left;
  background-image: url("./../assets/hero/hero_1.jpg");
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  background-attachment: fixed;
  position: relative;

  @media screen and (max-width: 834px) {
    height: 75vh;
  }
}

&::before {
  content: "";
  // Overlay should occupy the full width and height of parent image container
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0) 0%,
    rgba(0, 0, 0, .2) 100%
  );
  z-index: 1;
}

.hero-content {
  width: 80rem;
  max-width: 75vw;
  margin: 12rem auto 0;
  color: #fff;
  z-index: 10;

  @media screen and (max-width: 1280px) {
    margin: 12rem 8% 0;
  }
}

.heading {
  font-size: 4rem;
  font-weight: 800;
  letter-spacing: -0.25rem;
  z-index: 10;

  @media screen and (max-width: 834px) {
    font-size: 3rem;
  }
}

.hero-text {
  margin-top: 2rem;

  @media screen and (max-width: 834px) {
    font-size: 0.75rem;
  }
}
</style>
