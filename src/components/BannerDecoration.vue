<template>
  <div>
    <!-- img decoration -->
    <img
      class="deco-1"
      src="@/assets/img/h-2-slider-img-12.png"
      alt="slider-img12"
    />
    <img
      class="deco-2"
      src="@/assets/img/h-2-slider-img-13.png"
      alt="slider-img13"
    />
    <img
      class="deco-3"
      src="@/assets/img/h-2-slider-img-14.png"
      alt="slider-img14"
    />
    <img
      class="deco-4"
      src="@/assets/img/h-2-slider-img-17.png"
      alt="slider-img17"
    />
    <img
      class="deco-5"
      src="@/assets/img/short-slider-rev-1-img-6.png"
      alt="slider-img6"
    />
    <img
      class="deco-6"
      src="@/assets/img/short-slider-rev-1-img-2.png"
      alt="slider-img2"
    />
  </div>
</template>

<script>
export default {
  name: "BannerDecorationComponent",
};
</script>

<style  scoped lang="scss">
.deco-1 {
  position: absolute;
  left: 0%;
  top: 55%;
}
.deco-2 {
  position: absolute;
  bottom: 0%;
  left: 5%;
}
.deco-3 {
  position: absolute;
  right: 5%;
  top: 0%;
}
.deco-4 {
  position: absolute;
  bottom: 0%;
  right: 0%;
}
.deco-5 {
  position: absolute;
  right: 0%;
  top: 15%;
}
.deco-6 {
  position: absolute;
  left: 0%;
  top: 0%;
}
</style>