<template>
  <Header />
  <Cards />
  <ShellInfo />
  <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import Cards from "./components/Cards.vue";
import ShellInfo from "./components/ShellInfo.vue";
import Footer from "./components/Footer.vue";
import "./assets/css/main.css";

export default {
  name: "App",
  components: {
    Header,
    Cards,
    ShellInfo,
    Footer,
  },
};
</script>

<style>
#app {
  text-align: center;
}
</style>
