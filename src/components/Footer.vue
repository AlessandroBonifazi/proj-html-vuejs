<template>
  <div class="container-fluid ab-footer-bg mt-5">
    <div class="row ab-h300 d-flex justify-content-center align-items-center">
      <!-- logo -->
      <div class="col-2 d-flex flex-column align-items-start">
        <img src="@/assets/img/logo-sidearea-1.png" alt="logo" />
        <span>Let's get creative</span>
      </div>

      <!-- contacts -->
      <div class="col-2 d-flex flex-column align-items-start">
        <span>{{ email }}</span>
        <span>{{ phone }}</span>
      </div>

      <!-- location -->
      <div class="col-2 d-flex flex-column align-items-start">
        <span>{{ address }}</span>
        <span>{{ city }}</span>
      </div>

      <!-- social -->
      <div class="col-2 d-flex flex-column align-items-start">
        <span class="mx-3">Stay in touch with us</span>
        <div class="social w-50 mt-2 d-flex justify-content-between">
          <a href="#"
            ><font-awesome-icon class="social-icon" icon="fa-brands fa-twitter"
          /></a>
          <a href="#"
            ><font-awesome-icon
              class="social-icon"
              icon="fa-brands fa-pinterest-p"
          /></a>
          <a href="#"
            ><font-awesome-icon
              class="social-icon"
              icon="fa-brands fa-facebook-f"
          /></a>
          <a href="#"
            ><font-awesome-icon
              class="social-icon"
              icon="fa-brands fa-linkedin-in"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
  props: {
    email: String,
    phone: String,
    address: String,
    city: String,
  },
};
</script>

<style scoped lang="scss">
.ab-footer-bg {
  background-color: #c0e1cf;
  .social-icon {
    font-size: 25px;
  }
  img {
    height: 40px;
  }
  span {
    margin: 5px;
    font-size: 16px;
  }
}
</style>
