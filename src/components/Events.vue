<template>
  <div class="container-fluid my-5">
    <div class="row d-flex justify-content-center my-5">
      <div class="col-3">
        <div class="card">
          <img
            src="@/assets/img/h-2-blog-img-1.jpg"
            class="card-img-top"
            alt="event-pic"
          />
          <div class="card-body">
            <h5 class="card-title">
              This way, loves: a detailed guide through new design
            </h5>
            <span><em>By Emily Fields</em></span>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card">
          <img
            src="@/assets/img/h-2-blog-img-2.jpg"
            class="card-img-top"
            alt="event-pic"
          />
          <div class="card-body">
            <h5 class="card-title">
              I try to give people a different way of looking art
            </h5>
            <span><em>By Emily Fields</em></span>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card">
          <img
            src="@/assets/img/h-2-blog-img-3.jpg"
            class="card-img-top"
            alt="event-pic"
          />
          <div class="card-body">
            <h5 class="card-title">
              Introduce Richard Laperriére of those amazing features
            </h5>
            <span><em>By Emily Fields</em></span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "EventsComponent",
};
</script>

<style scoped lang="scss">
.card {
  border: none;
}
</style>
