<template>
  <div class="container-fluid my-5">
    <div class="row ab-h500 d-flex justify-content-center my-5">
      <!-- arrow slide -->
      <div class="col-1 d-flex justify-content-end align-items-center">
        <button @click="slideLeft()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-left" />
        </button>
      </div>

      <!-- Slide -->
      <div v-if="bannerID === 0" class="col-4 d-flex flex-column">
        <h1>Devotion that never ends</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="w-25">READ MORE</button>
      </div>
      <div v-if="bannerID === 0" class="col-4">
        <img src="@/assets/img/h-2-slider-img-15.png" alt="slider-img1" />
        <img src="@/assets/img/h-2-slider-img-16.png" alt="slider-img1" />
      </div>

      <!-- Slide -->
      <div v-if="bannerID === 1" class="col-4 d-flex flex-column">
        <h1></h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="w-25">READ MORE</button>
      </div>
      <div v-if="bannerID === 1" class="col-4">
        <img
          src="@/assets/img/short-slider-rev-1-img-3.png"
          alt="slider-img1"
        />
      </div>

      <!-- Slide -->
      <div v-if="bannerID === 2" class="col-4 d-flex flex-column">
        <h1>dajeeee</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          perspiciatis. Modi aliquam nisi deleniti rerum?
        </p>
        <button class="w-25">READ MORE</button>
      </div>
      <div v-if="bannerID === 2" class="col-4">
        <img src="@/assets/img/h-2-slider-img-11.png" alt="slider-img1" />
      </div>

      <!-- arrow slide -->
      <div class="col-1 d-flex align-items-center">
        <button @click="slideRight()" class="ab-arrow">
          <font-awesome-icon id="arrow-left" icon="fa-solid fa-angle-right" />
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerComponent",
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
</style>