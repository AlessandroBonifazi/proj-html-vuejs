<template>
  <div class="container-fluid">
    <div class="row">
      <ProductsComponent />
      <WorkProcessComponent />
      <ContactUsComponent />
      <EventsComponent />
    </div>
  </div>
</template>

<script>
import ProductsComponent from "./Products.vue";
import WorkProcessComponent from "./WorkProcess.vue";
import ContactUsComponent from "./ContactUs.vue";
import EventsComponent from "./Events.vue";

export default {
  name: "MainComponent",
  components: {
    ProductsComponent,
    WorkProcessComponent,
    ContactUsComponent,
    EventsComponent,
  },
};
</script>

<style scoped lang="scss">
</style>
