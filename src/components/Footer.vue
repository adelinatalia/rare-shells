<template>
  <footer :style="bgImg">
    <!-- <p><span>O.N</span>atalia</p> -->
  </footer>
</template>

<script>
export default {
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("@/assets/images/meer-strand.png")})`,
        backgroundRepeat: "no-repeat",
        backgroundSize: "cover",
      },
    };
  },
};
</script>

<style>
footer {
  height: 55vh;
  /* background-image: url("../assets/images/meer-strand.png"); */
}
</style>