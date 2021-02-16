<template>
  <div class="p-0">
    <div class="carousel-container">
      <b-carousel
        id="carousel-1"
        v-model="slide"
        indicators
        :interval="5000"
        background="#ababab"
      >
        <b-carousel-slide :img-src="require('@/assets/img/slider-img.png')">
          <h1 class="title-carousel">{{ title }}</h1>
          <h4 class="subtitle-carousel">
            {{ subtitle }}
          </h4>
          <div class="mt-4">
            <span @click="scroll('carousel-2')">
              <img
                class="clickable"
                :src="require('@/assets/icons/arrow-down.png')"
              />
            </span>
          </div>
        </b-carousel-slide>
        <b-carousel-slide :img-src="require('@/assets/img/slider-img.png')">
          <h1 class="title-carousel">{{ title }}</h1>
          <h4 class="subtitle-carousel">
            {{ subtitle }}
          </h4>
          <div class="mt-4">
            <span @click="scroll('carousel-2')">
              <img
                class="clickable"
                :src="require('@/assets/icons/arrow-down.png')"
              />
            </span>
          </div>
        </b-carousel-slide>
        <b-carousel-slide :img-src="require('@/assets/img/slider-img.png')">
          <h1 class="title-carousel">{{ title }}</h1>
          <h4 class="subtitle-carousel">
            {{ subtitle }}
          </h4>
          <div class="mt-4">
            <span @click="scroll('carousel-2')">
              <img
                class="clickable"
                :src="require('@/assets/icons/arrow-down.png')"
              />
            </span>
          </div>
        </b-carousel-slide>
      </b-carousel>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      title: "LOREM IPSUM",
      subtitle: "Lorem ipsum dolor sti amet, consectetur adipiscing elit"
    };
  },
  computed: {
    iconUrl() {
      return require("@/assets/icons/carousel-slider.png");
    }
  },
  methods: {
    scroll(id) {
      document.getElementById(id).scrollIntoView({
        behavior: "smooth"
      });
    }
  }
};
</script>

<style lang="css">
.title-carousel {
  color: #4d6128;
  font-weight: bold;
}
.subtitle-carousel {
  color: #213800;
  font-weight: bold;
}
.carousel-caption {
  top: 2rem;
}
.clickable {
  cursor: pointer;
}

#carousel-1___BV_indicators_ {
  height: 92px;
  background-color: rgba(49, 49, 49, 0.5);
  margin: 0;
}
#carousel-1___BV_indicator_1_,
#carousel-1___BV_indicator_2_,
#carousel-1___BV_indicator_3_ {
  list-style-type: none;
  background-image: url("../assets/icons/carousel-slider.png");
  background-color: transparent;
  height: 52px;
  width: 52px;
  outline: none;
  border-top: 25px solid transparent;
  border-bottom: 0;
}
#carousel-1___BV_indicator_1_.active,
#carousel-1___BV_indicator_2_.active,
#carousel-1___BV_indicator_3_.active {
  list-style-type: none;
  background-image: url("../assets/icons/carousel-slider-active.png");
  background-color: transparent;
  height: 52px;
  width: 52px;
  outline: none;
}
</style>
