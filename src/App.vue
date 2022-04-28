<template>
  <div id="app">
    <Header
      link1="HOME"
      link2="PAGES"
      link3="PORTFOLIO"
      link4="BLOG"
      link5="SHOP"
      link6="ELEMENTS"
    />
    <Banner />
    <Main />
    <Footer :email="email" :phone="phone" :address="address" :city="city" />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Banner from "./components/Banner.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Banner,
    Main,
    Footer,
  },
  data() {
    return {
      email: "maree.qode@gmail.com",
      phone: "+44645 321 789",
      address: "Avenue d'Auderghem 10",
      city: "1040 Brussels, Belgium",
    };
  },
};
</script>

<style lang="scss">
@import "@/style/general.scss";
@import "@/style/variables.scss";
@import "~bootstrap";
</style>
