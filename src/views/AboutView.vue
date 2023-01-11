<template>
  <div id="about">
    <div class="section-overlay">
      <h2 data-aos="zoom-in">About Me</h2>
      <div class="container-fluid container-lg about-container" data-aos="fade-right">
        <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" loading="lazy" class="profile-img about-img d-block">
          <div class="about-text bevel" data-aos="fade-left">
            <h5 data-aos="zoom-in">Who am I?</h5>
            <p data-aos="zoom-in" class="scroll">
              I am an ambitious and hardworking person who enjoys working with others. I enjoy learning new things and often spend time reading/watching tutorials to expand my knowledge or practising new skills that I find interesting.
              I am a hard-worker and I try my best to always be honest and reliable. I am often approached by colleagues when they need assistance and I generally enjoy helping them where I can. Even when I do not have the time to help others I still often find it difficult say no. In my spare time, I enjoy reading books, and playing chess.
              <br>
              <br>
              I have always been fascinated by the idea of 'coding'. The idea that some genius could get a computer to do whatever he wanted, with just a few lines of code, fascinated me. It almost seems unreal when I see my own code preforming it's magic before my eyes. This is why I am aspiring to become a professional developer.
              <br>
              <br>
            </p>
            <div class="cv-btns"  data-aos="zoom-in">
              <a href="./assets/CV (John-Bruce Noad).pdf" target="_blank"><button class="cv-open bevel">
                View CV
              </button></a>
              <a href="./assets/CV (John-Bruce Noad).pdf" download><button class="cv-download bevel">
                Download CV
              </button></a>
            </div>    
          </div>
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
/* About */
#about .section-overlay {
  padding-bottom: 20px;
}
.about-container {
  display: grid !important;
  grid-template-columns: repeat(3, 1fr) !important;
}
.about-img {
  grid-column: 1/2 !important;
}
.about-text {
  grid-column: 2/-1;
  width: auto;
  margin-left: 10px;
  padding: 15px 30px;
  background-color: var(--primaryColor);
  border-radius: 10px;
  min-height: 450px;
}
.about-text p {
  max-height: 300px !important;
}

.profile-img {
  border-radius: 10px;
  box-shadow: 0 0 15px black;
  margin: 0 5px;
}
#about .profile-img {
  max-width: 300px;
}

/* About (End) */

.cv-btns {
  grid-column: 1/-1;
}
.cv-open {
  background-color: darkcyan;
  margin: 10px;
  padding: 5px;
  font-weight: bold;
}
.cv-download {
  background-color: crimson;
  margin: 10px;
  padding: 5px;
  font-weight: bold;
}
.cv-open:hover {
  scale: 1.05;
  background-image: var(--primaryLinearGradient);
}
.cv-download:hover {
  scale: 1.05;
  background-image: var(--primaryLinearGradient);
}
.cv-open:active {
  scale: 0.9;
}
.cv-download:active {
  scale: 0.9;
}

.scroll {
  overflow-y: hidden;
  -webkit-mask-image: linear-gradient(to bottom, black 75%, transparent 100%);
  mask-image: linear-gradient(to bottom, black 75%, transparent 100%);
}
.scroll::-webkit-scrollbar {
  width: 10px;
}
.scroll::-webkit-scrollbar-track {
  background-color: #fff;
  border-radius: 50px;
}
.scroll::-webkit-scrollbar-thumb {
  background-image: var(--primaryLinearGradient);
  border-radius: 50px;
}
.scroll:hover {
  overflow-y: auto;
}


@media only screen and (max-width: 720px) {
  #home .profile-img {
    width: 300px;
    height: 300px;
  }

  #about {
    padding-bottom: 40px;
  }
  .about-img {
    grid-column: 1/-1 !important;
    margin: 10px auto;
  }
  .about-text {
    grid-column: 1/-1;
    margin-top: 20px;
  }
}

@media only screen and (max-width: 400px) {
  #about img, #home img {
    margin: auto;
    /* width: 85%; */
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
  #about {
    /* width: 20px; */
    word-wrap: break-word;
    word-break: break-all;
  }
}
</style>