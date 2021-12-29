<template>
  <Header />
  <Cards />
</template>

<script>
import Header from "./components/Header.vue";
import Cards from "./components/Cards.vue";
import "./assets/css/main.css";

export default {
  name: "App",
  components: {
    Header,
    Cards,
  },
};
</script>

<style>
#app {
  text-align: center;
}
</style>
