<template>
  <div :class="this.which" class="main">
    <Row :which="first" />
    <Row :which="second" />
    <Row :which="third" />
  </div>
</template>

<script>
import Row from "./row.vue";

export default {
  name: "Board",
  props: {
    which: String
  },
  components: {
    Row
  },
  computed: {
    first: function() {
      return (2 * (parseInt(this.which) - 1) + 1).toString();
    },
    second: function() {
      return (2 * (parseInt(this.which) - 1) + 2).toString();
    },
    third: function() {
      return (2 * (parseInt(this.which) - 1) + 3).toString();
    }
  }
};
</script>
