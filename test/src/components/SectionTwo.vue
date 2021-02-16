<template>
  <div class="p-0 main-div">
    <b-carousel id="carousel-2" v-model="slide" controls background="#ababab" :interval="0">
      <b-carousel-slide>
        <template v-slot:img>
          <div class="card-slider">
            <b-card-group>
              <div class="py-0 px-4">
                <b-card
                  :img-src="require('@/assets/img/slider-multiple-img.png')"
                  overlay
                >
                </b-card>
                <div class="text-slider">
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
                  </h6>
                </div>
              </div>
            </b-card-group>
          </div>
        </template>
      </b-carousel-slide>
      <b-carousel-slide>
        <template v-slot:img>
          <div class="card-slider">
            <b-card-group>
              <div class="py-0 px-4">
                <b-card
                  :img-src="require('@/assets/img/slider-multiple-img.png')"
                  overlay
                >
                </b-card>
                <div class="text-slider">
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
                  </h6>
                </div>
              </div>
            </b-card-group>
          </div>
        </template>
      </b-carousel-slide>
      <b-carousel-slide>
        <template v-slot:img>
          <div class="card-slider">
            <b-card-group>
              <div class="py-0 px-4">
                <b-card
                  :img-src="require('@/assets/img/slider-multiple-img.png')"
                  overlay
                >
                </b-card>
                <div class="text-slider">
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
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
                  <h4 class="title-slider">LOREM IPSUM</h4>
                  <h6>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmo tempor incididunt ut labore et dolore magna
                    aliqua. Quis ipsum suspendisse ultrices gravida. Risus
                    commodo viverra maecenas accumsan lacus vel facilisis.
                  </h6>
                </div>
              </div>
            </b-card-group>
          </div>
        </template>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
    };
  },
};
</script>

<style lang="css">
.main-div {
  background-color: #434343;
  height: 35rem;
}
.card-slider {
  background-color: #434343;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 35rem;
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

.card {
  border: 12px solid rgb(112, 112, 112) !important;
}

.carousel-control-prev, .carousel-control-next {
  bottom: 10rem!important;
  outline: none;
}

.carousel-control-prev-icon {
  background-image: url("../assets/icons/carousel-left.png")!important;
  width: 54px!important;
  height: 37px!important;
}

.carousel-control-next-icon {
  background-image: url("../assets/icons/carousel-right.png")!important;
  width: 54px!important;
  height: 37px!important;
}
</style>
