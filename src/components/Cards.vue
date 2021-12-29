<template>
  <section class="cards" v-for="shell in shells" :key="shell.id">
    <div class="card">
      <h2>{{ shell.name }}</h2>
      <img
        :src="require(`@/assets/${shell.img}`)"
        :alt="shell.name"
        width="200"
      />
      <p>{{ shell.description }}</p>
    </div>
  </section>
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
.cards {
  width: 100vw;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.card {
  width: 30vw;
  margin: 1rem;
  padding: 1rem 1.5rem;
  background-color: #fff;
  border-radius: 5px;
}

.card h2 {
  padding: 1rem 0;
  color: var(--primary);
}

.card p {
  padding-bottom: 2rem;
  line-height: 1.5em;
  color: var(--txt);
}

.card img {
  margin: 1rem 0;
}
</style>