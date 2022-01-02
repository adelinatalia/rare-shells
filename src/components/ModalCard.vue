<template>
  <div class="backdrop" @click="closeModal">
    <div class="modal">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ["toggleModal", "shells"],
  methods: {
    closeModal() {
      this.$emit("close");
    },
  },
};
</script>

<style scoped>
.backdrop {
  position: fixed;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
}
.modal {
  width: 50vw;
  margin: 1rem auto;
  padding: 1rem;
  border-radius: 10px;
  background: rgb(252, 249, 249);
}
@media only screen and (max-width: 930px) {
  .modal {
    width: 95vw;
  }
}
</style>