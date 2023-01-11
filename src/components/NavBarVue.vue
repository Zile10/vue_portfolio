<template lang="">
  <nav class="text-dark">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/projects">Projects</router-link> |
    <router-link to="/resume">Resume</router-link> |
    <router-link to="/testimonials">Testimonials</router-link> |
    <router-link to="/contact">Contact</router-link>
  </nav>
</template>
<script>
export default {
  
}
</script>
<style scoped>
  nav {
    box-shadow: 0 0 10px 0px black;
    word-wrap: break-word;
  }

  a {
    text-decoration: none;
  }
</style>