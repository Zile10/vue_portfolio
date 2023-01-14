<template>
  <NavBar/>
  <router-view/>
  <FooterVue/>
</template>

<script>
import NavBar from './components/NavBarVue.vue'
import FooterVue from './components/FooterVue.vue'

export default{
  components: {
    NavBar,
    FooterVue
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #2c3e50; */
  color: #fff;
}

:root{
  --navHeight: 100px;
  --primaryBoxShadow: 4px 4px 6px black;
  --bevel:   box-shadow:  inset 0.2em 0.2em 0.2em 0 rgba(200,200,200,0.5), inset -0.2em -0.2em 0.2em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --bevel2:  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --primaryColor: #333333;
  --secondaryColor: darkcyan;
  --primaryLinearGradient: linear-gradient(45deg, #42b983, #6bff2c);
  --secondaryColorInverted: #6bff2c;
}

.section-overlay{
  padding: 10px 0 20px;
  background: rgba(17, 17, 17, 0.63);
}

body{
  background-color: #222;
  scroll-margin-right: 100px;
  overflow-x: hidden;
}
body::-webkit-scrollbar {
  width: 15px;
  border-radius: 50px;
  background-color: #222;
}
body::-webkit-scrollbar-track {
  background-color: #555;
  border-radius: 50px;
  border: 1px solid darkviolet;
}
body::-webkit-scrollbar-thumb {
  background-image: var(--primaryLinearGradient);
  border-radius: 50px;
  border: 1px solid black;
  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5);
}
div#home, div#about, div#projects, div#resume, div#testimonials, div#contact {
  width: 100%;
  /* min-height: calc(100vh - var(--navHeight)); */
  scroll-margin-top: 100px;

  /* background-image: url('../assets/img/top-view-dark-modern-workplace-open-laptop.jpg'); */
  background-attachment: fixed;
  background-size: cover;
}

h1, h2, h3, h4 {
  text-shadow: var(--primaryBoxShadow);
}

.bevel {
  box-shadow:  inset 0.2em 0.2em 0.2em 0 rgba(200,200,200,0.5), inset -0.2em -0.2em 0.2em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
}

.bevel2 {
  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
}

/* Animation */
@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  50% {
    transform: rotate(180deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
/* Animation (End) */
</style>