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
@import url('https://fonts.googleapis.com/css2?family=Comfortaa&family=Sono&family=Space+Grotesk&display=swap');

:root{
  --navHeight: 100px;
  --primaryBoxShadow: 4px 4px 6px black;
  --bevel:   box-shadow:  inset 0.2em 0.2em 0.2em 0 rgba(200,200,200,0.5), inset -0.2em -0.2em 0.2em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --bevel2:  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --colorPrimary: #232328dd;
  --colorSecondary: #fff;
  --textColorPrimary: crimson;
  --textColorSecondary: #43AA8B;
  --primaryLinearGradient: linear-gradient(45deg, #B9B8D3, #B9B8D3);
  --secondaryColorInverted: #6bff2c;
  --font1: 'space grotesk';
  --font2: 'comfortaa';
  --font3: 'sono';
}
#app {
  font-family: var(--font1);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}
button {
  color: var(--colorSecondary);
}
button:hover {
  color: var(--colorPrimary);
}
p {
  font-family: var(--font2);
  font-size: 15px;
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
  width: 8px;
}
body::-webkit-scrollbar-track {
  background-color: #ddd;
  border-radius: 50px;
}
body::-webkit-scrollbar-thumb {
  background-color: var(--textColorPrimary);
  border-radius: 50px;
  /* box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5); */
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
  /* 25% {
    transform: rotate(90deg);
  }
  50% {
    transform: rotate(180deg);
  }
  75% {
    transform: rotate(270deg);
  } */
  100% {
    transform: rotate(360deg);
  }
}
/* Animation (End) */
</style>