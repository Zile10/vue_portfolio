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

@media only screen and (max-width: 720px) {
  #home .profile-img {
    width: 100px;
    height: 100px;
  }

  #about {
    padding-bottom: 40px;
  }
  .about-img {
    grid-column: 1/-1;
    margin: 10px auto;
  }
  .about-text {
    grid-column: 1/-1;
    margin-top: 20px;
  }

  .education-block p {
    grid-column: 1/-1;
  }
  .education-block h5, .education-block h6 {
    grid-column: 1/-1;
  }
  .education-block strong {
    color: #fff !important;
  };

  .skills-block {
    height: 550px;
    margin-bottom: 40px;
  }
  .html-skill {
    grid-column: 1/-1;
  }
  .css-skill {
    grid-column: 1/-1;
  }
  .javascript-skill {
    grid-column: 1/-1;
  }
  .bootstrap-skill {
    grid-column: 1/-1;
  }
  .excel-skill {
    grid-column: 1/-1;
  }
  .soft-skills {
    grid-column: 1/-1;
  }
}

@media only screen and (max-width: 400px) {
  #about img, #home img {
    margin: auto;
    width: 85%;
  }
  #home .profile-img {
    width: 250px;
    height: 250px;
  }
  #about .about-container {
    display: flex;
    flex-direction: column;
  }
  .about-text .cv-btns {
    margin-bottom: 10px;
    font-size: 15px;
  }
  .skills-block {
    width: 90%;
  }
  .project-card {
    width: 90%;
  }
  h2 {
    font-size: 2.5rem;
  }
}

@media only screen and (max-width: 300px) {
  h2 {
    font-size: 2rem;
  }
  #home .profile-img {
    width: 200px;
    height:  200px;
  }
  .footer-items {
    flex-direction: column;
  }
}

@media only screen and (max-width: 200px) {
  #home .profile-img {
    width: 150px;
    height: 150px;
  }
  .logo-link {
    display: none;
  }
  .skills-block {
    width: 95%;
  }
  h2 {
    font-size: 1.5rem;
  }
}
</style>