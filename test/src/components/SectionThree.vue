<template>
  <div class="p-0 h-32 main-div">
    <div class="row h-32 mx-0">
      <div class="col-6 center-flex">
        <div class="border-img mt-5per">
        <b-img
          v-bind="mainProps"
          rounded="circle"
          :src="require('@/assets/img/circle-img.png')"
        ></b-img>
        </div>
      </div>
      <div class="col-6 left-flex flex-column">
        <div class="paragraphs mt-5per">
          <h2><strong>LOREM IPSUM</strong></h2>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo
            tempor incididunt ut labore et dolore magna aliqua. Quis ipsum
            suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan
            lacus vel facilisis.
          </p>
          <p>
            <strong>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo
            tempor incididunt ut labore et dolore magna aliqua. Quis ipsum
            suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan
            lacus vel facilisis.
            </strong>
          </p>
          <p>
            <em>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo
            tempor incididunt ut labore et dolore magna aliqua. Quis ipsum
            suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan
            lacus vel facilisis.
            </em>
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo
            tempor incididunt ut labore et dolore magna aliqua. Quis ipsum
            suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan
            lacus vel facilisis.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mainProps: {
        blankColor: "#fff",
        width: 388,
        height: 388,
        class: "m1",
        center: true,
      },
    };
  },
};
</script>

<style>
.main-div {
  background-color: #707070;
}

.h-32 {
  height: 35rem;
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

h2, p {
  text-align: left;
  color: white;
}
.paragraphs {
  margin-right: 25%;
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

.mt-5per {
  margin-top: 5%;
}
</style>