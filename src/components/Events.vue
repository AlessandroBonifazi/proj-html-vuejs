<template>
  <div class="container-fluid my-5">
    <div class="row d-flex justify-content-center my-5">
      <!-- card -->
      <div class="col-3">
        <div class="card">
          <!-- img -->
          <img
            src="@/assets/img/h-2-blog-img-1.jpg"
            class="card-img-top"
            alt="event-pic"
          />

          <!-- date -->
          <div class="date">
            <div class="day">07</div>
            <div class="year">MAY '19</div>
          </div>

          <!-- details -->
          <div class="card-body">
            <h5 class="card-title">
              This way, loves: a detailed guide through new design
            </h5>
            <span><em>By Emily Fields</em></span>
          </div>
        </div>
      </div>

      <!-- card -->
      <div class="col-3">
        <div class="card">
          <!-- img -->
          <img
            src="@/assets/img/h-2-blog-img-2.jpg"
            class="card-img-top"
            alt="event-pic"
          />

          <!-- date -->
          <div class="date">
            <div class="day">13</div>
            <div class="year">MAY '19</div>
          </div>

          <!-- details -->
          <div class="card-body">
            <h5 class="card-title">
              I try to give people a different way of looking art
            </h5>
            <span><em>By Emily Fields</em></span>
          </div>
        </div>
      </div>

      <!-- card -->
      <div class="col-3">
        <div class="card">
          <!-- img -->
          <img
            src="@/assets/img/h-2-blog-img-3.jpg"
            class="card-img-top"
            alt="event-pic"
          />

          <!-- date -->
          <div class="date">
            <div class="day">21</div>
            <div class="year">MAY '19</div>
          </div>

          <!-- details -->
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
@import "@/style/variables.scss";

.card {
  border: none;
  position: relative;
  .card-body {
    h5 {
      font-size: 30px;
      font-weight: 600;
    }
    span {
      font-size: 18px;
      font-weight: 600;
    }
  }
  .date {
    position: absolute;
    top: -20px;
    left: 25px;
    text-align: center;
    .day {
      font-family: "Rouge Script", cursive;
      background-color: $bg-color3;
      font-size: 40px;
      font-weight: 700;
    }
    .year {
      padding: 10px;
      background-color: $bg-color2;
      font-weight: 700;
      .triangle {
        height: 0;
        width: 0;
        line-height: 0;
        border-bottom: 20px solid white;
        border-left: 20px solid transparent;
        border-right: 20px solid transparent;
      }
    }
  }
}
</style>
