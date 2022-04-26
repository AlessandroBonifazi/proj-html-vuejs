<template>
  <div class="container-fluid my-5">
    <div class="row">
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-1.jpg" alt="product-img-1" />
      </div>
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-2.jpg" alt="product-img-2" />
      </div>
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-3.jpg" alt="product-img-3" />
      </div>
    </div>

    <div class="row">
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-4.jpg" alt="product-img-4" />
      </div>
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-5.jpg" alt="product-img-5" />
      </div>
      <div class="col-4 p-0 m-0">
        <img src="@/assets/img/h-2-port-img-6.jpg" alt="product-img-6" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductsComponent",
  props: {
    msg: String,
  },
};
</script>

<style scoped lang="scss">
img {
  width: 100%;
}
</style>