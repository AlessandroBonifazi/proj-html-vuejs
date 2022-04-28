<template>
  <div class="container-fluid my-5">
    <div class="row mt-5">
      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-1.jpg" alt="product-img-1" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>

      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-2.jpg" alt="product-img-2" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>

      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-3.jpg" alt="product-img-3" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>
    </div>

    <div class="row mb-5">
      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-4.jpg" alt="product-img-4" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>

      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-5.jpg" alt="product-img-5" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>

      <!-- product -->
      <div class="col-4 position-relative imgHover p-0 m-0">
        <img src="@/assets/img/h-2-port-img-6.jpg" alt="product-img-6" />
        <div class="description">
          <h3>Illustration of novels</h3>
          <p><em>Illustration</em></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductsComponent",
};
</script>

<style scoped lang="scss">
.imgHover:hover .description {
  opacity: 1;
}
.description {
  position: absolute;
  top: 50%;
  left: 0%;
  transform: translate(-0%, -50%);
  opacity: 0;
  background-color: white;
  padding: 30px;
  width: 45%;
}
img {
  width: 100%;
}
</style>