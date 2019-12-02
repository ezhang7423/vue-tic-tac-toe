<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Row which="1" />
  </div>
</template>

<script>
import Row from "./components/row.vue";

export default {
  name: "app",
  components: {
    Row
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
