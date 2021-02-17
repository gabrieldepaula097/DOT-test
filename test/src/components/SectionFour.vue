<template>
  <div
    class="p-0 div-main"
    :class="{ 'h-35': this.openTab === 0, 'h-50rem': this.openTab > 0 }"
  >
    <div
      class="row mx-0"
      :class="{ 'h-35': this.openTab === 0, 'h-50rem': this.openTab > 0 }"
    >
      <div class="col-12 center-flex">
        <div class="accordion accordion-alt" role="tablist">
          <b-card no-body class="">
            <b-card-header
              header-tag="header"
              class="p-0 first mb-1px"
              :class="{ 'border-bottom-0': this.openTab === 1 }"
              role="tab"
            >
              <b-button
                block
                v-b-toggle.accordion-1
                variant="primary"
                class="justified-flex first"
                :class="{
                  'accordion-button': this.openTab !== 1,
                  'accordion-button-open': this.openTab === 1
                }"
                v-on:click="changeTab(1)"
                >{{ buttonText }}
                <img
                  v-if="this.openTab !== 1"
                  :src="require('@/assets/icons/arrow-accordion-collapsed.png')"
                  alt=""/>
                <img
                  v-if="this.openTab === 1"
                  :src="require('@/assets/icons/arrow-accordion-open.png')"
                  alt=""
              /></b-button>
            </b-card-header>
            <b-collapse
              id="accordion-1"
              visible
              accordion="my-accordion"
              role="tabpanel"
            >
              <b-card-body>
                <div class="row">
                  <div class="col-4">
                    <img
                      class="border-img-accordion"
                      :src="require('@/assets/img/accordion-img.png')"
                    />
                  </div>
                  <div class="col-8 center-flex">
                    <b-card-text>{{ text }}</b-card-text>
                  </div>
                </div>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="">
            <b-card-header
              header-tag="header"
              class="p-0 rounded-0 mb-1px"
              :class="{ 'border-bottom-0': this.openTab === 2 }"
              role="tab"
            >
              <b-button
                block
                v-b-toggle.accordion-2
                variant="primary"
                class="justified-flex"
                :class="{
                  'accordion-button': this.openTab !== 2,
                  'accordion-button-open': this.openTab === 2
                }"
                v-on:click="changeTab(2)"
                >{{ buttonText }}
                <img
                  v-if="this.openTab !== 2"
                  :src="require('@/assets/icons/arrow-accordion-collapsed.png')"
                  alt=""/>
                <img
                  v-if="this.openTab === 2"
                  :src="require('@/assets/icons/arrow-accordion-open.png')"
                  alt=""
              /></b-button>
            </b-card-header>
            <b-collapse
              id="accordion-2"
              accordion="my-accordion"
              role="tabpanel"
            >
              <b-card-body>
                <div class="row">
                  <div class="col-4">
                    <img
                      class="border-img-accordion"
                      :src="require('@/assets/img/accordion-img.png')"
                    />
                  </div>
                  <div class="col-8 center-flex">
                    <b-card-text>{{ text }}</b-card-text>
                  </div>
                </div>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="">
            <b-card-header
              header-tag="header"
              class="p-0 rounded-0 mb-1px"
              :class="{ 'border-bottom-0': this.openTab === 3 }"
              role="tab"
            >
              <b-button
                block
                v-b-toggle.accordion-3
                variant="primary"
                class="justified-flex"
                :class="{
                  'accordion-button': this.openTab !== 3,
                  'accordion-button-open': this.openTab === 3
                }"
                v-on:click="changeTab(3)"
                >{{ buttonText }}
                <img
                  v-if="this.openTab !== 3"
                  :src="require('@/assets/icons/arrow-accordion-collapsed.png')"
                  alt=""/>
                <img
                  v-if="this.openTab === 3"
                  :src="require('@/assets/icons/arrow-accordion-open.png')"
                  alt=""
              /></b-button>
            </b-card-header>
            <b-collapse
              id="accordion-3"
              accordion="my-accordion"
              role="tabpanel"
            >
              <b-card-body>
                <div class="row">
                  <div class="col-4">
                    <img
                      class="border-img-accordion"
                      :src="require('@/assets/img/accordion-img.png')"
                    />
                  </div>
                  <div class="col-8 center-flex">
                    <b-card-text>{{ text }}</b-card-text>
                  </div>
                </div>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="">
            <b-card-header
              header-tag="header"
              class="p-0 rounded-0 mb-1px"
              :class="{ 'border-bottom-0': this.openTab === 4 }"
              role="tab"
            >
              <b-button
                block
                v-b-toggle.accordion-4
                variant="primary"
                class="justified-flex"
                :class="{
                  'accordion-button': this.openTab !== 4,
                  'accordion-button-open': this.openTab === 4
                }"
                v-on:click="changeTab(4)"
                >{{ buttonText }}
                <img
                  v-if="this.openTab !== 4"
                  :src="require('@/assets/icons/arrow-accordion-collapsed.png')"
                  alt=""/>
                <img
                  v-if="this.openTab === 4"
                  :src="require('@/assets/icons/arrow-accordion-open.png')"
                  alt=""
              /></b-button>
            </b-card-header>
            <b-collapse
              id="accordion-4"
              accordion="my-accordion"
              role="tabpanel"
            >
              <b-card-body>
                <div class="row">
                  <div class="col-4">
                    <img
                      class="border-img-accordion"
                      :src="require('@/assets/img/accordion-img.png')"
                    />
                  </div>
                  <div class="col-8 center-flex">
                    <b-card-text>{{ text }}</b-card-text>
                  </div>
                </div>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="">
            <b-card-header
              header-tag="header"
              class="p-0 last"
              :class="{ 'border-bottom-0': this.openTab === 5 }"
              role="tab"
            >
              <b-button
                block
                v-b-toggle.accordion-5
                variant="primary"
                class="justified-flex last"
                :class="{
                  'accordion-button': this.openTab !== 5,
                  'accordion-button-open': this.openTab === 5
                }"
                v-on:click="changeTab(5)"
                >{{ buttonText }}
                <img
                  v-if="this.openTab !== 5"
                  :src="require('@/assets/icons/arrow-accordion-collapsed.png')"
                  alt=""/>
                <img
                  v-if="this.openTab === 5"
                  :src="require('@/assets/icons/arrow-accordion-open.png')"
                  alt=""
              /></b-button>
            </b-card-header>
            <b-collapse
              id="accordion-5"
              accordion="my-accordion"
              role="tabpanel"
            >
              <b-card-body>
                <div class="row">
                  <div class="col-4">
                    <img
                      class="border-img-accordion"
                      :src="require('@/assets/img/accordion-img.png')"
                    />
                  </div>
                  <div class="col-8 center-flex">
                    <b-card-text>{{ text }}</b-card-text>
                  </div>
                </div>
              </b-card-body>
            </b-collapse>
          </b-card>
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
      openTab: 1,
      buttonText: "Lorem ipsum",
      text:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmo tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis."
    };
  },
  methods: {
    changeTab(id) {
      if (this.openTab === id) {
        this.openTab = 0;
      } else {
        this.openTab = id;
      }
    }
  }
};
</script>

<style lang="css">
.div-main {
  background-color: #bfbfbf;
}

.accordion-alt {
  width: 85vw;
}

.accordion-alt .card {
  border: 0 !important;
}

.accordion-alt p {
  color: #707070;
}

.accordion-button-open {
  color: #707070 !important;
  background-color: #fff !important;
  border-color: #fff !important;
  height: 82px !important;
  padding-left: 10px !important;
  padding-right: 10px !important;
  border-top-left-radius: 0 !important;
  border-top-right-radius: 0 !important;
  border-bottom-right-radius: 0 !important;
  border-bottom-left-radius: 0 !important;
  font-weight: bold !important;
}

.accordion-button-open:focus,
.accordion-button:focus {
  outline: none !important;
  box-shadow: none !important;
}

.accordion-button {
  color: #fff !important;
  background-color: #707070 !important;
  border-color: #707070 !important;
  height: 82px !important;
  padding-left: 10px !important;
  padding-right: 10px !important;
  border-top-left-radius: 0 !important;
  border-top-right-radius: 0 !important;
  border-bottom-right-radius: 0 !important;
  border-bottom-left-radius: 0 !important;
  font-weight: bold !important;
}

.first {
  border-bottom-right-radius: 0 !important;
  border-bottom-left-radius: 0 !important;
}
.last {
  border-top-left-radius: 0 !important;
  border-top-right-radius: 0 !important;
  border-bottom-right-radius: 0.25rem !important;
  border-bottom-left-radius: 0.25rem !important;
}

.mb-1px {
  margin-bottom: 0.5px !important;
}

.border-img-accordion {
  border: 12px solid rgb(112, 112, 112);
}
</style>
