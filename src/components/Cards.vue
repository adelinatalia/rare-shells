<template>
  <div class="cards-container">
    <section class="cards">
      <div class="card" v-for="shell in shells" :key="shell.id">
        <h2>{{ shell.name }}</h2>
        <div class="img">
          <img
            :src="require(`@/assets/${shell.img}`)"
            :alt="shell.name"
            width="200"
          />
        </div>
        <div class="txt">
          <p>{{ shell.description }}</p>
        </div>
        <button class="btn btn-more">read more</button>
      </div>
    </section>
  </div>
</template>

<script>
import data from "../assets/data.json";

export default {
  data() {
    return {
      shells: data,
    };
  },
};
</script>

<style>
.cards-container {
  width: 100vw;
}

.cards {
  margin: 0 auto;
  width: 85vw;
  display: flex;
  flex-direction: row;
  align-items: center;
  flex-wrap: wrap;
  margin-top: -5rem;
}

.card {
  width: 25vw;
  height: 70vh;
  margin: 1rem;
  padding: 1rem 1.5rem;
  background-color: #fff;
  border-radius: 5px;
}

.card h2 {
  padding: 1rem 0;
  color: var(--primary);
}

.card .txt {
  height: 19vh;
}

.card p {
  padding-bottom: 2rem;
  line-height: 1.5em;
  color: var(--txt);
}

.card .img {
  margin: 1rem auto;
  width: 12vw;
  height: 17vh;
}

.card .img img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

/* big screen */
@media only screen and (min-width: 1400px) {
  .card {
    width: 25vw;
    height: 50vh;
  }

  .card .txt {
    height: 10vh;
  }
}

/* tablet */
@media only screen and (max-width: 930px) {
  .cards {
    margin-top: -10rem;
    width: 100vw;
    justify-content: space-around;
  }

  .card {
    width: 42vw;
    height: 43vh;
  }

  .card .img {
    width: 18vw;
    height: 17vh;
    margin: 0 auto;
  }

  .card .txt {
    height: 10vh;
  }
}

/* smart phone */
@media only screen and (max-width: 550px) {
  .card {
    width: 85vw;
    height: 50vh;
  }

  .card .img {
    width: 45vw;
    height: 17vh;
    margin: 0.5rem auto;
  }

  .card .txt {
    height: 11vh;
  }
}
</style>