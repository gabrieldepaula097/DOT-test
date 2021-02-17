<template>
  <div id="app">
    <SectionOne :checkMobile="checkMobile" />
    <SectionTwo :checkMobile="checkMobile" />
    <SectionThree :checkMobile="checkMobile" />
    <SectionFour :checkMobile="checkMobile" />
    <SectionFive :checkMobile="checkMobile" />
    <Footer :checkMobile="checkMobile" />
  </div>
</template>

<script>
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";
import SectionFour from "./components/SectionFour.vue";
import SectionFive from "./components/SectionFive.vue";
import Footer from "./components/Footer.vue";
import { checkMobile } from "@/helpers/checkMobile.js";

export default {
  name: "App",
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    Footer
  },
  data() {
    return {
      checkMobile: null,
    }
  },
  mounted() {
    this.checkMobile = checkMobile();
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
  background-color: transparent;
}
.h-30 {
  height: 30rem;
}

.h-35 {
  height: 35rem;
}
.h-40 {
  height: 40rem;
}
.h-50rem {
  height: 50rem;
}

.h-66 {
  height: 66%;
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

.w-100vw {
  width: 100vw!important;
}
</style>
