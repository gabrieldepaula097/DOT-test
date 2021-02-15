<template>
  <div id="app">
    <SectionOneTwo />
  </div>
</template>

<script>
import SectionOneTwo from "./components/SectionOneTwo.vue";

export default {
  name: "App",
  components: {
    SectionOneTwo
  }
};
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: black;
}
</style>
