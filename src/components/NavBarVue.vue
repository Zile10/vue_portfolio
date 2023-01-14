<template lang="">
  <nav class="text-dark">
    <router-link to="/" class="logo-link animate__animated animate__bounce animate__delay-1s">
      <img class="logo" src="https://i.postimg.cc/RVMYyxKL/INTJ-white.png" alt="">
    </router-link>    

    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/resume">Resume</router-link> |
    <router-link to="/projects">Projects</router-link> |
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
    padding: 30px;
  }

  nav a {
    font-weight: bold;
    color: white;
  }
  nav a:hover {
    font-weight: bold;
    color: #6bff2c;
  }

  nav a.router-link-exact-active {
    color: #42b983 !important;
  }

  nav {
    box-shadow: 0 0 10px 0px black;
    word-wrap: break-word;
    padding: 15px;
  }
  .logo {
    /* filter: invert(100%); */
    width: 90px;
    border-radius: 60px;
    box-shadow: 0 0 6px 2px black;
    scale: 1;
    margin-right: 20px;
  }
  .logo:hover {
    scale: 1.05;
    background-image: var(--primaryLinearGradient);
    animation: 1s linear spin infinite;
    animation-fill-mode: forwards;
  }


  a {
    text-decoration: none;
  }

  @media only screen and (max-width: 300px) {
    .logo-link {
      display: none;
    }
  }

</style>