<template>
  <div class="container-fluid my-5 ab-contact-bg">
    <div class="row mt-5">
      <div
        class="
          col-10
          offset-1
          d-flex
          flex-column
          align-items-center
          text-center
        "
      >
        <h1>
          Want to work with us? Send us <strong><em>a message!</em></strong>
        </h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique
          nulla dolor voluptatum delectus alias dolorem ipsa laudantium eum
          reiciendis sunt. Similique nulla dolor voluptatum delectus alias
          dolorem ipsa laudantium eum reiciendis sunt.
        </p>
        <button class="ab-btn">CONTACT</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactUsComponent",
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

.ab-contact-bg {
  background-image: url("@/assets/img/h-2-background-1.jpg");
  background-size: contain;
  padding: 80px;
  h1 {
    font-size: 80px;
    margin-bottom: 30px;
  }
  p {
    color: $p-color;
    font-size: 23px;
  }
  .ab-btn {
    border: 4px solid $bg-color1;
    background-color: $bg-color1;
  }
  .ab-btn:hover {
    color: black;
    border: 4px solid $bg-color1;
    background-color: white;
  }
}
</style>