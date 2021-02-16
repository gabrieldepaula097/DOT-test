<template>
  <div id="app">
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
  </div>
</template>

<script>
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";
import SectionFour from "./components/SectionFour.vue";

export default {
  name: "App",
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour
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

.h-35 {
  height: 35rem;
}

.h-45 {
  height: 45rem;
}
.center-flex {
  display: flex;
  align-items: center;
  justify-content: center;
}

.left-flex {
  display: flex;
  align-items: baseline;
  justify-content: center;
}

.justified-flex {
  display: flex !important;
  align-items: center;
  justify-content: space-between;
}
</style>
