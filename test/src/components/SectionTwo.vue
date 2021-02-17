<template>
  <div class="p-0 main-div h-35">
    <b-carousel
      id="carousel-2"
      v-model="slide"
      controls
      :interval="5000"
      background="#ababab"
    >
      <div v-if="!checkMobile">
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>{{ text }}</h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
      </div>
      <div v-if="checkMobile">
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <div class="card-slider h-35">
              <b-card-group>
                <div class="py-0 px-4">
                  <b-card
                    :img-src="require('@/assets/img/slider-multiple-img.png')"
                    overlay
                  >
                  </b-card>
                  <div class="text-slider">
                    <h4 class="title-slider">{{ title }}</h4>
                    <h6>
                      {{ text }}
                    </h6>
                  </div>
                </div>
              </b-card-group>
            </div>
          </template>
        </b-carousel-slide>
      </div>
    </b-carousel>
  </div>
</template>

<script>
import { checkMobile } from "@/helpers/checkMobile.js";

export default {
  data() {
    return {
      checkMobile: null,
      slide: 0,
      title: "LOREM IPSUM",
      text:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis."
    };
  },
  mounted() {
    this.checkMobile = checkMobile();
  }
};
</script>

<style lang="css">
.card-slider {
  background-color: #434343;
  display: flex;
  justify-content: center;
  align-items: center;
}
.card {
  border: 12px solid rgb(112, 112, 112) !important;
}
.carousel-control-prev,
.carousel-control-next {
  bottom: 10rem !important;
  outline: none;
}

.carousel-control-prev-icon {
  background-image: url("../assets/icons/carousel-left.png") !important;
  width: 54px !important;
  height: 37px !important;
}

.carousel-control-next-icon {
  background-image: url("../assets/icons/carousel-right.png") !important;
  width: 54px !important;
  height: 37px !important;
}
.title-slider {
  color: white;
  font-weight: bold;
  margin-top: 1rem;
}
.text-slider {
  top: 2rem;
  width: 20rem;
}
.text-slider h6 {
  color: white;
  font-weight: 600;
}
/* smartphones, portrait iPhone, portrait 480x320 phones (Android) */
@media (min-width: 320px) and (max-width: 479px) {
  .carousel-control-prev,
  .carousel-control-next {
    top: 90% !important;
    width: 70% !important;
  }
}

@media (min-width: 1025px) and (max-width: 1280px) {
  #carousel-2 .carousel-control-prev {
    width: 85px !important;
  }
  #carousel-2 .carousel-control-next {
    width: 85px !important;
  }
}
</style>
<style lang="css" scoped>
.main-div {
  background-color: #434343;
}
</style>
