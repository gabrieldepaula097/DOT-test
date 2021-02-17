<template>
  <div class="p-0 main-div" :class="{ 'h-35': !this.checkMobile }">
    <div class="row mx-0" :class="{ 'h-35': !this.checkMobile }">
        <div class="col-6 center-flex" v-if="!checkMobile">
          <div class="border-img mt-5per">
            <b-img
              v-bind="mainProps"
              rounded="circle"
              :src="require('@/assets/img/circle-img.png')"
            ></b-img>
          </div>
        </div>
        <div class="col-6 left-flex flex-column" v-if="!checkMobile">
          <div class="paragraphs mt-5per">
            <h2>
              <strong>{{ title }}</strong>
            </h2>
            <p>
              {{ text }}
            </p>
            <p>
              <strong>
                {{ text }}
              </strong>
            </p>
            <p>
              <em>
                {{ text }}
              </em>
            </p>
            <p>
              {{ text }}
            </p>
          </div>
        </div>
      <div v-if="checkMobile">
        <div class="col-12 center-flex p-0">
          <img
            class="w-100vw"
            :src="require('@/assets/img/circle-img-mobile.png')"
          />
        </div>
        <div class="col-12 center-flex flex-column">
          <div class="title-three">
            <h2>
              <strong>{{ title }}</strong>
            </h2>
          </div>
          <div class="text-three">
            <p>
              {{ text }}
            </p>
            <p>
              <strong>
                {{ text }}
              </strong>
            </p>
            <p>
              <em>
                {{ text }}
              </em>
            </p>
            <p>
              {{ text }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["checkMobile"],
  data() {
    return {
      mainProps: {
        blankColor: "#fff",
        width: 388,
        height: 388,
        center: true,
      },
      title: "LOREM IPSUM",
      text:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis.",
    };
  },
};
</script>

<style lang="css">
h2,
p {
  text-align: left;
  color: white;
}
.main-div {
  background-color: #707070;
}
.paragraphs {
  margin-right: 25%;
}
.mt-5per {
  margin-top: 5%;
}
.border-img {
  border-radius: 100%;
  display: flex;
  flex: 0 0 427px;
  height: 428px;
  justify-content: center;
  overflow: hidden;
  position: relative;
  width: 428px;
  border: 20px solid #313131;
}

/* smartphones, portrait iPhone, portrait 480x320 phones (Android) */
@media (min-width: 320px) and (max-width: 599px) {
  h2,
  p {
    text-align: center;
    color: white;
  }

  .title-three {
    position: relative;
    bottom: 3rem;
  }

  .text-three {
    position: relative;
    bottom: 1.5rem;
  }
}
</style>
