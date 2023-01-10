<template lang="">
  <div class="card project-card bevel col-12 col-sm-4 col-md-3 bg-dark">
    <h3 data-aos="zoom-in"><br> {{ title }} </h3>
    <a :href="siteUrl" target="_blank" data-aos="zoom-in">
      <img :src="imgSrc" alt="" class="project-preview">
    </a>
    <p data-aos="zoom-in">
      {{ description }}
    </p>
    <div class="btns d-flex justify-content-evenly" data-aos="zoom-in">
      <form :action="githubRepo" method="get" target="_blank">
        <button class="project-btn github bevel2" type="submit">GitHub</button>
      </form>
      <form :action="siteUrl" method="get" target="_blank">
        <button class="project-btn netlify bevel2" type="submit">Netlify</button>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  props: ['title', 'siteUrl', 'githubRepo', 'imgSrc', 'description']
}
</script>
<style lang="">
  
</style>