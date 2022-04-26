<template>
  <Products />
</template>

<script>
import Products from "./Products.vue";
export default {
  name: "MainComponent",
  components: {
    Products,
  },
  props: {
    msg: String,
  },
};
</script>

<style scoped lang="scss">
</style>
