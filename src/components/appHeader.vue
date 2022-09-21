<template>
  <div>
    <div>
      <div class="app--header">
        <AppNav class="" />
      </div>
      <div>
        <div id="carouselExampleFade" class="carousel slide carousel-fade" data-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active" data-interval="5000">
                <img src="@/assets/img/11.jpg" class="d-block w-100 animate__animated animate__zoomIn" alt="...">
                </div>

                <div class="carousel-item" data-interval="5000">
                <img src="@/assets/img/12.jpg" class="d-block w-100 animate__animated animate__zoomIn" alt="...">
                </div>

                <div class="carousel-item" data-interval="5000">
                <img src="@/assets/img/13.jpg" class="d-block w-100 animate__animated animate__zoomIn" alt="...">
                </div>

                <div class="carousel-item" data-interval="5000">
                <img src="@/assets/img/14.jpg" class="d-block w-100 animate__animated animate__zoomIn" alt="...">
                </div>

                <div class="carousel-item" data-interval="5000">
                <img src="@/assets/img/15.jpg" class="d-block w-100 animate__animated animate__zoomIn" alt="...">
                </div>
               
            </div>
            <button class="carousel-control-prev" type="button" data-target="#carouselExampleFade" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-target="#carouselExampleFade" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </button>
        </div>
        <div class="hero--carousel"></div>
      </div>
    </div>
  </div>
</template>

<script>
import items from "@/plugins/images.js";
import AppNav from "./appNav.vue";
export default {
  data() {
    return {
      images: items,
    }
  },
  components: { AppNav },
};
</script>