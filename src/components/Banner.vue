<template>
  <div class="container-fluid my-5">
    <div class="row ab-h550 d-flex justify-content-center my-5">
      <!-- arrow slide -->
      <div class="col-1 d-flex justify-content-end align-items-center">
        <button @click="slideLeft()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-left" />
        </button>
      </div>

      <!-- Slide -->
      <div
        v-if="bannerID === 0"
        class="col-3 d-flex flex-column justify-content-center"
      >
        <h1>Devotion that never ends</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="ab-btn">READ MORE</button>
      </div>
      <div v-if="bannerID === 0" class="col-4 position-relative">
        <img src="@/assets/img/h-2-slider-img-15.png" alt="slider-img1" />
        <img src="@/assets/img/h-2-slider-img-16.png" alt="slider-img1" />

        <BannerDecorationComponent />
      </div>

      <!-- Slide -->
      <div
        v-if="bannerID === 1"
        class="col-3 d-flex flex-column justify-content-center"
      >
        <h1>Get inspired</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="ab-btn">READ MORE</button>
      </div>
      <div
        v-if="bannerID === 1"
        class="col-4 d-flex justify-content-center position-relative"
      >
        <img
          src="@/assets/img/short-slider-rev-1-img-3.png"
          alt="slider-img1"
        />

        <BannerDecorationComponent />
      </div>

      <!-- Slide -->
      <div
        v-if="bannerID === 2"
        class="col-3 d-flex flex-column justify-content-center"
      >
        <h1>We love our work</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="ab-btn">READ MORE</button>
      </div>
      <div v-if="bannerID === 2" class="col-4 position-relative">
        <img src="@/assets/img/h-2-slider-img-11.png" alt="slider-img1" />

        <BannerDecorationComponent />
      </div>

      <!-- arrow slide -->
      <div class="col-1 d-flex align-items-center">
        <button @click="slideRight()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-right" />
        </button>
      </div>
    </div>

    <div class="row d-flex justify-content-center">
      <div class="col-1 d-flex">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>
    </div>
  </div>
</template>

<script>
import BannerDecorationComponent from "./BannerDecoration.vue";

export default {
  name: "BannerComponent",
  components: {
    BannerDecorationComponent,
  },
  data() {
    return {
      bannerID: 0,
    };
  },
  methods: {
    slideLeft() {
      if (this.bannerID === 0) {
        return this.bannerID;
      } else {
        let activeID = this.bannerID;
        this.bannerID = this.bannerID - 1;
        console.log(activeID);
      }
    },
    slideRight() {
      if (this.bannerID === 2) {
        return this.bannerID;
      } else {
        let activeID = this.bannerID;
        this.bannerID = this.bannerID + 1;
        console.log(activeID);
      }
    },
  },
};
</script>

<style scoped lang="scss">
.ab-arrow {
  height: 50px;
  width: 50px;
  border: none;
  border-radius: 50%;
  font-size: 20px;
  transition: 0.6s ease;
  background-color: white;
}
.ab-arrow:hover {
  background-color: rgba(0, 0, 0, 0.103);
}
.dot {
  cursor: pointer;
  height: 14px;
  width: 14px;
  margin: 0 5px;
  background-color: #e1c0b0;
  border-radius: 50%;
}
</style>