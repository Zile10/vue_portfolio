<template>
  <div class="card testimonial-card bevel2 my-2 col-11 col-sm-7 col-lg-3 my-4" data-aos="fade-up-left">
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

  <ModalVue :name="name" :imgSrc="imgSrc" :quote="quote"/>
</template>

<script>
// import CardVue from './CardVue.vue'
import ModalVue from '@/components/ModalVue.vue'
export default {
  components: {
    // CardVue,
    ModalVue
  },
  props: ['imgSrc', 'name', 'surname', 'quote']
}
</script>

<style scoped>
  .testimonial-card {
    background-color: var(--colorPrimary)
  }
  .testimonial-picture {
    width: 90%;
    height: 200px;
    object-fit: cover;
    object-position: top;
    margin: 10px auto;
    border-radius: 15px;
  }
  .modal .testimonial-picture {
    width: 70%;
    height: 300px;
    object-fit: cover;
    object-position: top;
    margin: 10px auto;
    border-radius: 15px;
  }

  h5, p {
    color: #ddd;
  }
</style>