<template>
  <div id="about">
    <div class="section-overlay">
      <h2 data-aos="zoom-in" class="animate__animated animate__bounceIn mt-2">About Me</h2>
      <div class="container-fluid container-lg about-container my-3 bevel" data-aos="fade-right">
        <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" class="profile-img about-img d-block">
          <div class="about-text" data-aos="fade-left">
            <h5 data-aos="zoom-in">Who am I?</h5> 
            <p data-aos="zoom-in" class="scroll">
              I am a young 19 year old young man, born and raised in Cape Town South Africa. I was raised in primarily Afrikaans family, with strong Christian values. I have, however, always been in english schools where I was surrounded by different cultures and beliefs. I attended Groote Schuur Primary (in english) for 7 years before attending Wynberg Boys High for the following 5. Still unsure about my future at that point, I decided to use the next year to figure things out. I already had an interest in code/programming at this point, with basic self-taUght knowledge on the topic, but during this year, this interest soared and through free online tutorials, I taught myself HTML, CSS, JavaScript and the basics NodeJS. I also began looking a little at mongoDB and Flutter, but at this point I had already discovered Life Choices and decided to join the academy.
            </p>
          </div>
          
          <div class="interests-text" data-aos="fade-in">
            <h5 data-aos="zoom-in">Hobbies and Interests:</h5> 
            <p data-aos="zoom-in" class="scroll">
              I enjoy learning and often spend my spare time up skilling by following along with coding tutorials or practising via my own coding projects and challenges. I also enjoy reading, especially non-fiction books. I particularly like the author 'Robert, Greene', who writes about concepts such as power, life/career strategies, and general self-improvement, which I am quite passionate about. I also enjoy playing chess as I find the game both challenging an stimulating. I began playing in high school, (although I had learn the basic rules, many years before) and quickly become absorbed in the game. I especially enjoyed competing against others for a position on the school's chess ladder, a ranking system for our chess players.
            </p>
          </div>

          <div class="strengths-text" data-aos="fade-in">
            <h5 data-aos="zoom-in">Strengths:</h5> 
            <p data-aos="zoom-in" class="scroll">
              I am a hardworking, passionate individual when it comes to my interests or the things I do. This is clear from the time I spend on my hobbies such as chess, reading and programming. 
              <br>
              I am proactive and driven, when it comes to working toward my goals. This is evident form the programming work and learning I did independently and without direction from others in order to better my future prospects in the field.
              <br>
              I am tenacious, as when I truly want something, I will stop at nothing to get it. This clearly displayed in my attitude towards the game of chess. Often I have found myself losing to tough opponents, but this is when I get truly excited to play again. I tend to replay against that opponent, again and again, until either I win, or they give in.
              <br>
              I am not only open to learning, but also thoroughly enjoy it. In chess, I believe the best opponent is one that is at least slightly stronger than yourself. This way, victory is within reach, but you still have to push yourself to grow in order to reach it. I enjoy reading and facing code based challenges for very much the same reason.
            </p>
          </div>

          <div class="cv-btns"  data-aos="zoom-in">
            <a href="https://drive.google.com/file/d/1DJbRrfjiwCsHI2xIkCYnIDgU8Q-KOd_S/view?usp=share_link" target="_blank"><button class="cv-open bevel">
              View CV
            </button></a>
            <!-- <a href="../assets/CV (John-Bruce Noad).pdf" download><button class="cv-download bevel">
              Download CV
            </button></a> -->
          </div>    
      </div>
    </div>
  </div>

  <!-- I am an ambitious and hardworking person who enjoys working with others. I enjoy learning new things and often spend time reading/watching tutorials to expand my knowledge or practising new skills that I find interesting.
  I am a hard-worker and I try my best to always be honest and reliable. I am often approached by colleagues when they need assistance and I generally enjoy helping them where I can. Even when I do not have the time to help others I still often find it difficult say no. In my spare time, I enjoy reading books, and playing chess.
  <br> -->
</template>

<script>


export default {
  name: 'HomeView',
  components: {
    // HelloWorld
  }
}
</script>

<style scoped>
/* About */
#about {
  background-image: url(https://i.postimg.cc/4dcKMWXH/jeshoots-com-unsplash-white-desk.jpg);
}
#about .section-overlay {
  padding-bottom: 20px;
}
.about-container {
  display: grid !important;
  grid-template-columns: repeat(4, 1fr) !important;
  /* grid-template-rows: 3fr 1fr; */
  background-color: var(--primaryColor);
  padding: 15px 30px;
  border-radius: 3px;
}
.about-img {
  grid-column: 1/2 !important;
  grid-row: 1/2 !important;
}
.about-text {
  grid-column: 2/-1;
  width: auto;
  /* margin-left: 10px; */
  /* min-height: 450px; */
}
.interests-text {
  grid-column: span 2;
}
.strengths-text {
  grid-column: span 2
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
  max-width: 240px;
  margin: 10px auto
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

@media only screen and (max-width: 1000px) {
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