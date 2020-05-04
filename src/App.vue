<template>
  <div id="app">
    <Header />
    <Hero />
    <List />
  </div>
</template>

<script>
import Header from "./components/shared/Header.vue";
import Hero from "./components/Hero.vue";
import List from "./components/List.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    List
  }
};
</script>

<style lang="less">
#app {
  font-family: "Poppins", Poppins, Helvetica Neue, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #000;
  display: flex;
  flex-direction: column;
}
</style>
