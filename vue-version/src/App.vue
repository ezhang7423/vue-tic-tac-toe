<template>
  <div id="app">
    <Logo />

    <div class="board-wrapper">
      <Board which="1" />
    </div>
  </div>
</template>

<script>
import Board from "./components/board.vue";
import Logo from "./components/logo.vue";
export default {
  name: "app",
  components: {
    Board,
    Logo
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #02060a;
  height: 100vh;
  background: rgb(236, 236, 216);
}

.board-wrapper {
  margin: auto;
  height: fit-content;
  width: fit-content;
  margin-top: 20vh;
  align-items: center;
  display: flex;
  flex-direction: column;
}
</style>
