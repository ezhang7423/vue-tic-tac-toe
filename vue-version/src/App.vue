<template id="app">
  <!-- doesn't work, want full background -->
  <div>
    <Logo />

    <div class="board-wrapper">
      <Board which="1" />

      <div class="hide play" onclick="location.reload();">Play again?</div>
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
  align-items: center;
  display: flex;
  flex-direction: column;
}
.hide {
  visibility: hidden;
}

.play {
  margin-top: 30px;
  background-color: #44c767;
  border-radius: 28px;
  border: 1px solid #18ab29;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: san-serif, "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS";
  font-size: 30px;
  padding: 16px 31px;
  text-decoration: none;
}

.play:hover {
  background-color: #5cbf2a;
}

.play:active {
  position: relative;
  top: 1px;
}
</style>
