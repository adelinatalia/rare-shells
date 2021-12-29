<template>
  <header id="header">
    <h1>
      6 Rare & Beautiful
      <br />
      Types of Shells
    </h1>
    <div id="hero-video">
      <video autoplay muted loop id="hero-video" height="950">
        <source src="../assets/images/meer.mp4" type="video/mp4" />
      </video>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
header {
  width: 100vw;
  height: 70vh;
}

#hero-video {
  width: 100vw;
  height: 70vh;
}

video {
  width: 100%;
  object-fit: cover;
  overflow: hidden;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

h1 {
  font-size: 5em;
  font-weight: bold;
  letter-spacing: 0.03em;
  color: transparent;
  -webkit-text-stroke-width: 3px;
  -webkit-text-stroke-color: #fff;
  position: relative;
  top: 5rem;
}

@media only screen and (max-width: 470px) {
  header h1 {
    top: 2rem;
    font-size: 4em;
  }
}
</style>
