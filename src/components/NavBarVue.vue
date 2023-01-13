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
    box-shadow: 0 0 10px 0px black;
    word-wrap: break-word;
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
    animation: 2s linear spin infinite;
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



<style>
/*
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark">
  <div class="container-fluid">
    <router-link to="/" class="logo-link animate__animated animate__bounce animate__delay-1s">
      <img class="logo" src="https://i.postimg.cc/RVMYyxKL/INTJ-white.png" alt="">
    </router-link>    
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse bg-dark p-1 rounded-1" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <router-link class="nav-link active" aria-current="page" to="/">
            <!-- <span class="material-symbols-outlined">home</span> -->
            Home
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" aria-current="page" to="/about">About</router-link>
        </li>

        <li class="nav-item dropdown">
          <router-link class="nav-link dropdown-toggle" to="/resume" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Work
          </router-link>
          <ul class="dropdown-menu bg-dark">
            <li><router-link class="dropdown-item text-light" to="/resume#education">Education</router-link></li>
            <li><router-link class="dropdown-item text-light" to="/resume#skills">Skills</router-link></li>
            <li><router-link class="dropdown-item text-light" to="/projects">Projects</router-link></li>
          </ul>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" aria-current="page" to="/testimonials">Testimonials</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" aria-current="page" to="/contact">Contact</router-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
*/

</style>
