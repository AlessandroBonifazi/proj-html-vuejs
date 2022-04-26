<template>
  <div class="container-fluid">
    <div class="row ab-h100 d-flex justify-content-between align-items-center">
      <!-- Logo -->
      <div class="col-1">
        <img src="@/assets/img/logo-sidearea-1.png" alt="logo-header" />
      </div>
      <!-- Nav -->
      <div class="col-5 d-flex justify-content-end">
        <ul class="nav">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Active</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link">Disabled</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Active</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Active</a>
          </li>
        </ul>
        <!-- Menu -->
        <div>
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
    msg: String,
  },
};
</script>

<style scoped lang="scss">
</style>
