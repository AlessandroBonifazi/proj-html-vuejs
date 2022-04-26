<template>
  <div id="app">
    <Header msg="Welcome to Your Vue.js App" />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "@/style/general.scss";
@import "@/style/variables.scss";
</style>
