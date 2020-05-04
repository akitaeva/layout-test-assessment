<template>
  <div class="top-bar">
    <div class="logo">
      <img src="@/assets/logo.png" />
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

<style scoped lang="less">
.top-bar {
  height: 3rem;
  width: 100%;
  max-width: 60rem;
  margin: 0 auto;
  padding-top: 1rem;
  display: flex;
  justify-content: space-between;
  background: transparant;
}

.nav-links {
  display: flex;
  justify-content: space-between;
  width: 28rem;
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
