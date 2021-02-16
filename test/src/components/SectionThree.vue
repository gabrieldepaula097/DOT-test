<template>
  <div class="p-0 h-35 main-div">
    <div class="row h-35 mx-0">
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
        center: true
      },
      title: "LOREM IPSUM",
      text:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis."
    };
  }
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
</style>
