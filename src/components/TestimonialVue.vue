<template>
  <div class="card testimonial-card bevel2 my-2 col-11 col-sm-7 col-lg-3 bg-dark my-4" data-aos="fade-up-left">
    <img :src="imgSrc" class="card-img-top testimonial-picture" alt="...">
    <div class="card-body">
      <h5 class="card-title">{{ name + ' ' + surname }}</h5>
      <div class="scroll">
        <p class="card-text">
          {{ quote }}
          <br>
          <br>
        </p>
      </div>
      <button class="btn btn-primary bevel" data-bs-toggle="modal" :data-bs-target="'#'+name+'-Modal'">View More</button>
    </div>
  </div>

  <!-- Modal -->
  <div class="modal fade" :id="name+'-Modal'" tabindex="-1" :aria-labelledby="name+'-Modal'" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content" style="background-color: transparent; ">
        <div class="modal-body bg-dark rounded-4">
          <div class="modal-header bg-dark">
            <h1 class="modal-title fs-5" id="exampleModalLabel">{{ name }}</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          
          <div class="card testimonial-card bg-dark w-100 h-100 my-2 my-4" data-aos="fade-right" style="border: none;">
            <img :src="imgSrc" class="card-img-top testimonial-picture" alt="...">
            <div class="card-body">
              <h5 class="card-title"></h5>
              <div class="">
                <p class="card-text">{{ quote }}</p>
              </div>
            </div>
          </div>        

          <button type="button" class="btn btn-secondary bevel" data-bs-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>
  <!-- Modal End -->

</template>

<script>
// import CardVue from './CardVue.vue'
export default {
  components: {
    // CardVue,
  },
  props: ['imgSrc', 'name', 'surname', 'quote']
}
</script>

<style scoped>
  h5, p {
    color: #ddd;
  }
</style>