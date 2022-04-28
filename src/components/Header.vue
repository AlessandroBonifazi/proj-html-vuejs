<template>
  <div class="container-fluid">
    <div class="row ab-h100 d-flex justify-content-between align-items-center">
      <!-- Logo -->
      <div class="col-1 mx-3">
        <img src="@/assets/img/logo-sidearea-1.png" alt="logo-header" />
      </div>
      <!-- Nav -->
      <div class="col-5 d-flex justify-content-end">
        <ul class="nav mx-5">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">{{ link1 }}</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">{{ link2 }}</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">{{ link3 }}</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">{{ link4 }}</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">{{ link5 }}</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">{{ link6 }}</a>
          </li>
        </ul>
        <!-- Menu -->
        <div class="ab-h23">
          <img src="@/assets/svg/svg-1.svg" alt="menu-button" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {
    link1: String,
    link2: String,
    link3: String,
    link4: String,
    link5: String,
    link6: String,
  },
};
</script>

<style scoped lang="scss">
.nav-item {
  border: 5px solid white;
}
.nav-item:hover {
  border-bottom: 5px solid #f0cebe;
}
</style>
