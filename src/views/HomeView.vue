<template>
  <div class="home">
    <div class="section-overlay">
        <h1 class="d-block intro" data-aos="zoom-in">Hi There</h1>
        <div class="d-block">
          <h4 data-aos="fade-left">I am John-Bruce Noad. Welcome to my page!</h4>
          <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" loading="lazy" class="profile-img" width="250px">
          <h5><strong>Aspiring Software & Web Developer</strong></h5>
        </div>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    // HelloWorld
  }
}
</script>

<style scoped>
  .profile-img {
    border-radius: 10px;
    box-shadow: 0 0 15px black;
    margin: 0 5px;
  }

</style>