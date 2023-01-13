<!-- eslint-disable vue/require-v-for-key -->
<template>
  <div id="projectCarousel" class="carousel slide h-50 w-100" data-bs-ride="false">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#projectCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#projectCarousel" :data-bs-slide-to="n" v-for="n in slides-1"  :aria-label="'Slide ' + (n+1)"></button>
      <!-- <button type="button" data-bs-target="#projectCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button> -->
    </div>
    <div class="carousel-inner w-100 h-100" data-aos="fade-up">

      <slot></slot>

    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#projectCarousel" data-bs-slide="prev">
      <span class="carousel-control-prev-icon text-light" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next text-light" type="button" data-bs-target="#projectCarousel" data-bs-slide="next">
      <span class="carousel-control-next-icon " aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script>
export default {
  props: ['slides'],
  data() {
    return {
      slidesArr: []
    }
  },
}
</script>

<style>
  #projectCarousel {
    z-index: 1;
  }
</style>