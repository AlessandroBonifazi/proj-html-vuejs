<template>
  <div class="container-fluid my-5">
    <div class="row mt-5">
      <!-- section title -->
      <div class="col-12 text-center">
        <h1>Working <em>process</em></h1>
      </div>
    </div>

    <div class="row">
      <div class="col-8 offset-2 ab-line-bg d-flex justify-content-around">
        <!-- frame -->
        <div class="frame d-flex align-items-center justify-content-center">
          <font-awesome-icon icon="fa-solid fa-lightbulb" class="ab-icons" />
        </div>

        <!-- frame -->
        <div class="frame d-flex align-items-center justify-content-center">
          <font-awesome-icon icon="fa-regular fa-comment" class="ab-icons" />
        </div>

        <!-- frame -->
        <div class="frame d-flex align-items-center justify-content-center">
          <font-awesome-icon icon="fa-solid fa-cloud" class="ab-icons" />
        </div>

        <!-- frame -->
        <div class="frame d-flex align-items-center justify-content-center">
          <font-awesome-icon icon="fa-solid fa-pencil" class="ab-icons" />
        </div>
      </div>
    </div>

    <div class="row mb-5">
      <div class="col-8 offset-2 d-flex justify-content-around">
        <!-- card -->
        <div class="ab-card d-flex flex-column align-items-center">
          <!-- card title -->
          <h3>First theres an idea</h3>
          <!-- text -->
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>

        <!-- card -->
        <div class="ab-card d-flex flex-column align-items-center">
          <!-- card title -->
          <h3>Then we talk about</h3>
          <!-- text -->
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>

        <!-- card -->
        <div class="ab-card d-flex flex-column align-items-center">
          <!-- card title -->
          <h3>And we think about</h3>
          <!-- text -->
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>

        <!-- card -->
        <div class="ab-card d-flex flex-column align-items-center">
          <!-- card title -->
          <h3>So we draw along</h3>
          <!-- text -->
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WorkProcessComponent",
};
</script>

<style scoped lang="scss">
h1 {
  font-size: 80px;
}
.ab-line-bg {
  background-image: url("@/assets/svg/svg-3.svg");
  background-repeat: no-repeat;
  background-clip: content-box;
  background-position: 50%;
  padding: 65px 0px 30px 0px;
}
.ab-card {
  width: 18%;
  text-align: center;
  h3 {
    font-size: 25px;
  }
}
.frame {
  height: 150px;
  width: 150px;
  border-radius: 50%;
  background-color: #faf7f1;
  .ab-icons {
    height: 30px;
  }
}
</style>