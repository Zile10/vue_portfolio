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
  --secondaryBoxShadow: 2px 2px 6px darkviolet;
  --bevel:   box-shadow:  inset 0.2em 0.2em 0.2em 0 rgba(200,200,200,0.5), inset -0.2em -0.2em 0.2em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --bevel2:  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
  --primaryColor: #333;
  --secondaryColor: darkviolet;
  --primaryLinearGradient: linear-gradient(45deg, darkviolet, crimson);
  --secondaryColorInverted: #6bff2c;
}

.section-overlay{
  padding: 10px 0 20px;
  background: rgba(128, 128, 128, 0.5);
  
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.bevel {
  box-shadow:  inset 0.2em 0.2em 0.2em 0 rgba(200,200,200,0.5), inset -0.2em -0.2em 0.2em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
}

.bevel2 {
  box-shadow:  inset 0.1em 0.1em 0.1em 0 rgba(200,200,200,0.5), inset -0.1em -0.1em 0.1em 0 rgba(0,0,0,0.5), 0 0 15px 2px black;
}
</style>