<template>
  <div class="top-bar">
    <div class="logo">
      <img src="@/assets/logo.png" alt="Logo" />
    </div>
    <div class="menu-bars">
      <img :src="menuBars" alt="menu" />
    </div>
    <div class="nav-links">
      <a href="/">
        About
      </a>
      <a href="/">
        Destinations
      </a>
      <a href="/">
        Book Now
      </a>
      <a href="/">
        <div class="sign-in-box">
          <img src="@/assets/icons/sign-in.svg" />
          Sign In
        </div>
      </a>
    </div>
  </div>
</template>

<script>
import menuBars from "@/assets/icons/menu-bars-outline.png";

export default {
  name: "Thumbnail",
  data() {
    return {
      menuBars: menuBars
    };
  }
};
</script>

<style scoped lang="less">
.top-bar {
  height: 3rem;
  width: 100%;
  max-width: 60rem;
  margin: 0 auto;
  padding-top: 1rem;
  display: flex;
  justify-content: space-between;
}

.nav-links {
  display: flex;
  justify-content: space-between;
  width: 28rem;
  margin-right: 1.5rem;

  @media screen and (max-width: 833px) {
    display: none;
  }
}

.logo {
  max-height: 3rem;
  margin-left: 1.5rem;
}

.menu-bars {
  max-height: 3rem;
  max-width: 3rem;
  margin-right: 1.5rem;

  img {
    height: 90%;
  }  

  @media screen and (min-width: 834px) {
    display: none;
  }
}

a {
  color: #fff;
  text-decoration: none;
  text-transform: uppercase;
}

.sign-in-box {
  display: flex;
  width: 6rem;
  justify-content: space-between;
}
</style>
