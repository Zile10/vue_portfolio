<template>
  <div id="projects">
    <div class="section-overlay">
      <h2 data-aos="zoom-in">Projects</h2>
      
      <Carousel slides="6">
        <div class="carousel-item active">
          <ProjectCard 
            title="Running Man Game!" 
            siteUrl="https://running-man-game.netlify.app/" 
            githubRepo="https://github.com/Zile10/runningManGame.git" 
            imgSrc="https://i.postimg.cc/hGFH4VWQ/running-Man-Game-preview.png" 
            description="To test my self-taught coding skills, one of my first practise projects was this 'Running Game'. Based on and inspired by Google Chrome's very own Dinosaur Game! Now with an incomplete menu! 😂"
          />
          <StarsAnimation/>
        </div>
  
        <div class="carousel-item">
          <ProjectCard 
            title="Canvas JS Bouncy Balls Simulation!" 
            siteUrl="https://canvas-bouncy-balls.netlify.app/" 
            githubRepo="https://github.com/Zile10/canvasBoucyBalls.git" 
            imgSrc="https://i.postimg.cc/tTd1vdy3/canvas-Boucy-Balls-preview.png" 
            description="After learning about canvas.js and all it could do, I began practising using it, by building a few basic simulations. This gravity simulation, was one of those first few simulation. Tip: Click anywhere to restart the simulation."
          />
          <BallsAnimation/>
        </div>
  
        <div class="carousel-item">
          <ProjectCard 
            title="Life Choices HTML/CSS Revision Project" 
            siteUrl="https://revision-dummy.netlify.app/" 
            githubRepo="https://github.com/Zile10/revision_day.git" 
            imgSrc="https://i.postimg.cc/FKD8y8k3/revision-site-preview.png" 
            description="A revision project I created during the Life Choices coding course, incorporating various HTML and CSS elements. This includes the use of flexbox, grid, media queries and various other elements used when creating a responsive webpage."
          />
          <DogAnimation/>
        </div>
  
        <div class="carousel-item">
          <ProjectCard 
            title="JS Calculator" 
            siteUrl="https://john-bruce-js-calculator.netlify.app/" 
            githubRepo="https://github.com/Zile10/calculator.git" 
            imgSrc="https://i.postimg.cc/Y9Cr8vg7/calculator-preview.png" 
            description="A calculator project I created during the LC Coding Course using JS. The display uses basic HTML and CSS. It can preform basic functions such ad addition subtraction multiplication and division, as well as slightly more complete functions suc as exponents and square roots, all while following the 'BODMAS' rule."
          />
          <MathAnimation/>
        </div>
  
        <div class="carousel-item">
          <ProjectCard 
            title="JS E-commerce Site " 
            siteUrl="https://john-bruce-js-eomp.netlify.app/" 
            githubRepo="https://github.com/Zile10/POS_system.git" 
            imgSrc="https://i.postimg.cc/t4q7B3f1/Ecom-preview.png" 
            description="An e-commerce site that I created during the LC Coding Course. With a complete and working products page, checkout system, and admin page, using the CRUD system! Data is stored in and fetched from the local storage."
          />
          <MoneyAnimation/>
        </div>
  
        <div class="carousel-item">
          <ProjectCard 
            title="HTML & CSS Portfolio" 
            siteUrl="https://john-bruce-portfolio.netlify.app/" 
            githubRepo="https://github.com/Zile10/portfolio.git" 
            imgSrc="https://i.postimg.cc/J4WskV55/portfolio-preview.png" 
            description="My original portfolio, created in the LC Coding course. This portfolio makes use of only HTML, CSS and a few related libraries, such as bootstrap and Animate On Scroll. I am quite proud of this design, and managed to score highly on this project! 😄"
          />
          <PortfolioAnimation/>
        </div>
      </Carousel>
    </div>
  </div>
</template>

<script>
import Carousel from '@/components/CarouselVue.vue'
import ProjectCard from '@/components/ProjectCard.vue'

import BallsAnimation from '@/components/animations/BallsAnimation.vue'
import StarsAnimation from '@/components/animations/StarsAnimation.vue'
import DogAnimation from '@/components/animations/DogAnimation.vue'
import MathAnimation from '@/components/animations/MathAnimation.vue'
import MoneyAnimation from '@/components/animations/MoneyAnimation.vue'
import PortfolioAnimation from '@/components/animations/PortfolioAnimation.vue'
export default {
  name: 'HomeView',
  components: {
    Carousel,
    ProjectCard,
    BallsAnimation,
    StarsAnimation,
    DogAnimation,
    MathAnimation,
    MoneyAnimation,
    PortfolioAnimation,
  },
  data() {
    return {
      projects: [
        {
          project: 'Running Man Game!',
          sitUrl: "https://running-man-game.netlify.app/",
          githubRepo:"https://github.com/Zile10/runningManGame.git",
          imgSrc:"https://i.postimg.cc/hGFH4VWQ/running-Man-Game-preview.png",
          description:"To test my self-taught coding skills, one of my first practise projects was this 'Running Game'. Based on and inspired by Google Chrome's very own Dinosaur Game! Now with an incomplete menu! 😂",
          animation: "StarsAnimation"
        },
        {
          project: "Canvas JS Bouncy Balls Simulation!",
          sitUrl: "https://canvas-bouncy-balls.netlify.app/",
          githubRepo: "https://github.com/Zile10/canvasBoucyBalls.git",
          imgSrc: "https://i.postimg.cc/tTd1vdy3/canvas-Boucy-Balls-preview.png",
          description: "After learning about canvas.js and all it could do, I began practising using it, by building a few basic simulations. This gravity simulation, was one of those first few simulation. Tip: Click anywhere to restart the simulation.",
          animation: "BallsAnimation"
        },
        {
          project: "Life Choices HTML/CSS Revision Project",
          sitUrl: "https://revision-dummy.netlify.app/",
          githubRepo: "https://github.com/Zile10/revision_day.git",
          imgSrc: "https://i.postimg.cc/FKD8y8k3/revision-site-preview.png",
          description: "A revision project I created during the Life Choices coding course, incorporating various HTML and CSS elements. This includes the use of flexbox, grid, media queries and various other elements used when creating a responsive webpage.",
          animation: "DogAnimation"
        },
        {
          project: "JS Calculator",
          sitUrl: "https://john-bruce-js-calculator.netlify.app/",
          githubRepo: "https://github.com/Zile10/calculator.git",
          imgSrc: "https://i.postimg.cc/Y9Cr8vg7/calculator-preview.png",
          description: "A calculator project I created during the LC Coding Course using JS. The display uses basic HTML and CSS. It can preform basic functions such ad addition subtraction multiplication and division, as well as slightly more complete functions suc as exponents and square roots, all while following the 'BODMAS' rule.",
          animation: "MathAnimation"
        },
        {
          project: "JS E-commerce Site",
          sitUrl: "https://john-bruce-js-eomp.netlify.app/",
          githubRepo: "https://github.com/Zile10/POS_system.git",
          imgSrc: "https://i.postimg.cc/t4q7B3f1/Ecom-preview.png",
          description: "An e-commerce site that I created during the LC Coding Course. With a complete and working products page, checkout system, and admin page, using the CRUD system! Data is stored in and fetched from the local storage.",
          animation: ""
        },
        {
          project: "HTML & CSS Portfolio",
          sitUrl: "https://john-bruce-portfolio.netlify.app/",
          githubRepo: "https://github.com/Zile10/portfolio.git",
          imgSrc: "https://i.postimg.cc/J4WskV55/portfolio-preview.png",
          description: "My original portfolio, created in the LC Coding course. This portfolio makes use of only HTML, CSS and a few related libraries, such as bootstrap and Animate On Scroll. I am quite proud of this design, and managed to score highly on this project! 😄",
          animation: ""
        },
      ]
    }
  },
}
</script>

<style>
#projects {
  background-image: url(https://i.postimg.cc/SsKq5rC7/top-view-dark-modern-workplace-open-laptop.jpg);
}
.project-card {
  min-height: 280px;
  width: 350px;
  margin: 1em;
  padding: 0 10px;
  border-radius: 5px;
  color: white;
  display: inline-block;
}
.project-card:hover {
  scale: 1.05;
}
.project-card p {
  padding: 0 5px;
}
.project-preview {
  width: 70%;
  border-radius: 10px;
  border: 1px solid black;
}
.project-preview:hover {
  scale: 1.05;
  border-color: #aaa;
}

.project-btn {
  background-color: #333;
  color: #fff;
  padding: 3px 5px;
  cursor: pointer;
  margin: auto;
  align-items: center;
  text-align: center;
  border: 1px solid black;
  text-shadow: 0 0 5px black;
  margin-bottom: 25px;
}
.project-btn.github {
  background-color: crimson;
}
.project-btn.netlify {
  background-color: darkcyan;
}
.project-btn:hover {
  border-color: var(--secondaryColor);
  background-image: var(--primaryLinearGradient);
  scale: 1.1;
}
.project-btn:active {
  scale: 0.9;
}

h1, h2, h3, h4, h5, h6, p{
  word-wrap: break-word;
  /* background-color: #ffffff4d; */
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