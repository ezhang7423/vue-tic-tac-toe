<template>
  <div class="vue-logo-wrapper">
    Made with
    <img class="vue" src="../assets/vue.svg" alt="vue logo" />
  </div>
</template>

<script>
export default {
  name: "Logo"
};
</script>

<style scoped>
.vue {
  width: 40vw;
}

@media (min-width: 600px) {
  .vue {
    width: 20vw;
  }
}

.vue-logo-wrapper {
  display: flex;
  align-items: center;
}
</style>