<template>
  <div class="section-overlay">
    <h2 data-aos="zoom-in">Projects</h2>
    
    <Carousel>
      <div class="carousel-item active">
        <ProjectCard 
          title="Running Man Game!" 
          siteUrl="https://running-man-game.netlify.app/" 
          githubRepo="https://github.com/Zile10/runningManGame.git" 
          imgSrc="https://i.postimg.cc/hGFH4VWQ/running-Man-Game-preview.png" 
          description="To test my self-taught coding skills, one of my first practise projects was this 'Running Game'. Based on and inspired by Google Chrome's very own Dinosaur Game! Now with an incomplete menu! 😂"
        />
      </div>

      <div class="carousel-item">
        <ProjectCard 
          title="Canvas JS Bouncy Balls Simulation!" 
          siteUrl="https://canvas-bouncy-balls.netlify.app/" 
          githubRepo="https://github.com/Zile10/canvasBoucyBalls.git" 
          imgSrc="https://i.postimg.cc/tTd1vdy3/canvas-Boucy-Balls-preview.png" 
          description="After learning about canvas.js and all it could do, I began practising using it, by building a few basic simulations. This gravity simulation, was one of those first few simulation. Tip: Click anywhere to restart the simulation."
        />
      </div>

      <div class="carousel-item">
        <ProjectCard 
          title="Life Choices HTML/CSS Revision Project" 
          siteUrl="https://revision-dummy.netlify.app/" 
          githubRepo="https://github.com/Zile10/revision_day.git" 
          imgSrc="https://i.postimg.cc/FKD8y8k3/revision-site-preview.png" 
          description="A revision project I created during the Life Choices coding course, incorporating various HTML and CSS elements. This includes the use of flexbox, grid, media queries and various other elements used when creating a responsive webpage."
        />
      </div>
    </Carousel>
  </div>
</template>

<script>
import Carousel from '@/components/CarouselVue.vue'
import ProjectCard from '@/components/ProjectCard.vue'
export default {
  name: 'HomeView',
  components: {
    Carousel,
    ProjectCard,
  }
}
</script>

<style>
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
</style>