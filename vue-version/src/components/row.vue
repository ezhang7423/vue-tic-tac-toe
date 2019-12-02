<template>
  <div :class="this.which" class="main">
    <Box :which="first" />
    <Box :which="second" />
    <Box :which="third" />
  </div>
</template>

<script>
import Box from "./box.vue";

export default {
  name: "row",
  props: {
    which: String
  },
  components: {
    Box
  },
  computed: {
    first: function() {
      return (3 * parseInt(this.which) - 2).toString();
    },
    second: function() {
      return (3 * parseInt(this.which) - 1).toString();
    },
    third: function() {
      return (3 * parseInt(this.which)).toString();
    }
  }
};
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: row;
}
</style>