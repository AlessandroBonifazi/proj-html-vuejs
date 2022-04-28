<template>
  <div class="container-fluid my-5">
    <div class="row ab-h550 d-flex justify-content-center my-5">
      <!-- arrow slide -->
      <div class="col-1 d-flex justify-content-end align-items-center mx-3">
        <button @click="slideLeft()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-left" />
        </button>
      </div>

      <!-- Slide -->
      <div
        v-if="bannerID === 0"
        class="col-3 d-flex flex-column justify-content-center"
      >
        <h1>Devotion that never <em>ends</em></h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="ab-btn">READ MORE</button>
      </div>
      <!-- imgs -->
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
      <!-- imgs -->
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
        <h1>We love our <em>work</em></h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="ab-btn">READ MORE</button>
      </div>
      <!-- imgs -->
      <div v-if="bannerID === 2" class="col-4 position-relative">
        <img src="@/assets/img/h-2-slider-img-11.png" alt="slider-img1" />

        <BannerDecorationComponent />
      </div>

      <!-- arrow slide -->
      <div class="col-1 d-flex align-items-center mx-3">
        <button @click="slideRight()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-right" />
        </button>
      </div>
    </div>

    <!-- slide dots -->
    <div class="row d-flex justify-content-center">
      <div v-if="bannerID === 0" class="col-1 d-flex align-items-center">
        <span class="dot active"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>

      <div v-if="bannerID === 1" class="col-1 d-flex align-items-center">
        <span class="dot"></span>
        <span class="dot active"></span>
        <span class="dot"></span>
      </div>

      <div v-if="bannerID === 2" class="col-1 d-flex align-items-center">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot active"></span>
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
        return (this.bannerID = 2);
      } else {
        let activeID = this.bannerID;
        this.bannerID = this.bannerID - 1;
        console.log(activeID);
      }
    },
    slideRight() {
      if (this.bannerID === 2) {
        return (this.bannerID = 0);
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
  font-size: 28px;
  transition: 0.5s ease;
  color: white;
  background-color: #e1c0b0;
}
.ab-arrow:hover {
  border: 3px solid black;
}
.ab-transition {
  transition: 0.5s ease;
}
.dot {
  cursor: pointer;
  height: 14px;
  width: 14px;
  margin: 0 5px;
  background-color: #e1c0b0;
  border-radius: 50%;
}
.active {
  height: 18px;
  width: 18px;
  border: 1px solid black;
}
h1 {
  font-size: 70px;
  font-weight: 600;
}
p {
  font-size: 18px;
}
</style>