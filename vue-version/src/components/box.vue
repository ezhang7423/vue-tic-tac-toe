<template>
  <div :class="this.which" class="col">
    <span class="fade-in is-paused"></span>
  </div>
</template>

<script>
export default {
  name: "box",
  props: {
    which: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.col {
  width: 8rem;
  height: 8rem;
  border: 1px solid black;
  font-size: 8rem;
  font-family: "Lato", "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS",
    sans-serif;
  text-align: center;
  align-content: center;
  line-height: 8rem;
}

@media only screen and (max-width: 600px) {
  .col {
    width: 5.7rem;
    height: 5.7rem;
    font-size: 5.7rem;
    line-height: 6rem;
  }
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

.fade-in {
  opacity: 0;
  animation: fadeIn 0.2s ease-out 1 forwards;
}

.is-paused {
  animation-play-state: paused;
}
</style>
