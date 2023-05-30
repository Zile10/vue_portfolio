<template>
  <div id="about">
    <div class="section-overlay">
      <h2 data-aos="zoom-in" class="animate__animated animate__bounceIn mt-2">
        About Me
      </h2>
      <div
        class="container-fluid container-lg about-container my-3"
        data-aos="fade-right"
      >
        <img
          src="https://i.postimg.cc/fy0p3Y9k/john-bruce-noad-portfolio-photo.jpg"
          alt="John-Bruce Profile"
          data-aos="fade-right"
          class="profile-img about-img d-block"
        />
        <div class="about-text text-block bevel" data-aos="fade-left">
          <h5 data-aos="zoom-in">Who am I?</h5>
          <p data-aos="zoom-in" class="scroll">
            I am a 19 year old, born and raised in Cape Town
            South Africa. I was raised in primarily Afrikaans family, with
            strong Christian values. I have, however, always been in english
            schools where I was surrounded by different cultures and beliefs. I
            attended Groote Schuur Primary (in english) for 7 years before
            attending Wynberg Boys High for the following 5. 
            <br><br>
            Still unsure about
            my future at that point, I decided to use the next year to figure
            things out. I already had an interest in code/programming at this
            point, with basic self-taught knowledge on the topic, but during
            this year, this interest soared and through free online tutorials, I
            taught myself HTML, CSS, JavaScript and the basics NodeJS. I also
            began looking a little at mongoDB and Flutter, but at this point I
            had already discovered Life Choices and decided to join the academy.
          </p>
          <div class="cv-btns" data-aos="zoom-in">
            <a
              href="https://drive.google.com/file/d/1ymc0mJ-2FW9eA9ZIVT8O0Auoe3NWWtVA/view?usp=sharing"
              target="_blank"
              ><button class="cv-open bevel">View CV</button></a
            >
            <a href="./John-Bruce Noad CV Resume.pdf" download><button class="cv-download bevel">
                Download CV
              </button></a>
          </div>
        </div>

        <div class="interests-text text-block bevel" data-aos="fade-in">
          <h5 data-aos="zoom-in">Hobbies and Interests:</h5>
          <p data-aos="zoom-in" class="scroll">
            I enjoy learning and often spend my spare time <span>up-skilling</span> by
            following along with coding tutorials or <span>practising</span> by doing <span>my own
            coding projects and challenges</span>. I also <span>enjoy reading</span>, especially
            non-fiction books. I particularly like the author 'Robert, Greene',
            who writes about concepts such as power, life/career strategies, and
            general <span>self-improvement</span>, which I am quite passionate about. 
            <br><br>
            I also enjoy <span>playing chess</span> as I find the game both challenging an
            stimulating. I began playing in high school, (although I had learn
            the basic rules, many years before) and quickly become absorbed in
            the game. I especially <span>enjoyed competing</span> against others for a
            position on the school's chess ladder, a ranking system for our
            chess players.
          </p>
        </div>

        <div class="strengths-text text-block bevel" data-aos="fade-in">
          <h5 data-aos="zoom-in">Strengths:</h5>
          <p data-aos="zoom-in" class="scroll">
            - I am a <span>hardworking, passionate</span> individual when it
            comes to my interests or the things I do. This is clear from the
            time I spend on my hobbies such as chess, reading and programming.
            <br>
            - I am <span>proactive and driven</span>, when it comes to working
            toward my goals. This is evident form the work and learning I did
            independently and without external direction.
            <br>
            - I am <span>tenacious</span>, as I will stop at nothing to get what
            I desire. This is best displayed in my attitude towards chess: When
            I face a tough opponent, I keep challenging them until I win.
            <br>
            - Lastly, I am not only <span>open to learning</span>, but also
            <span>thoroughly enjoy it</span>, as shown by all of my previous
            examples.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
  components: {
    
  },
};
</script>

<style scoped>
/* About */
#about {
  background-image: url(https://i.postimg.cc/4dcKMWXH/jeshoots-com-unsplash-white-desk.jpg);
  padding-bottom: 0 !important;
}
.about-container {
  display: grid !important;
  grid-template-columns: repeat(4, 1fr) !important;
  gap: 10px;
}
.about-img {
  grid-column: 1/2 !important;
  grid-row: 1/2 !important;
}
.about-text {
  grid-column: 2/-1;
  width: auto;
  margin-left: 10px;
}
.interests-text,
.strengths-text {
  grid-column: span 2;
  width: auto;
  margin: 20px 5px;
}
.text-block p {
  padding-bottom: 25px;
}
.text-block {
  background-color: var(--colorPrimary);
  padding: 15px 30px;
  border-radius: 3px;
}
span {
  color: var(--textColorSecondary);
  font-weight: bold;
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
  margin: 10px auto;
}

/* About (End) */

.cv-btns {
  grid-column: 1/-1;
}
.cv-open {
  background-color: var(--textColorSecondary);
  text-shadow: 0 0  2px black;
  margin: 10px;
  padding: 5px;
  font-weight: bold;
}
.cv-download {
  background-color: var(--textColorPrimary);
  margin: 10px;
  padding: 5px;
  font-weight: bold;
}
.cv-open:hover {
  scale: 1.05;
  background-image: var(--primaryLinearGradient);
  text-shadow: none;
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
  -webkit-mask-image: linear-gradient(to bottom, black 90%, transparent 100%);
  mask-image: linear-gradient(to bottom, black 90%, transparent 100%);
  padding: 10px;
  padding-bottom: 25px;
  max-height: 300px;
}
.scroll::-webkit-scrollbar {
  width: 10px;
}
.scroll::-webkit-scrollbar-track {
  background-color: #fff;
  border-radius: 50px;
}
.scroll::-webkit-scrollbar-thumb {
  background-color: var(--textColorPrimary);
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
  .interests-text, .strengths-text {
    grid-column: 1/-1;
  }
}

@media only screen and (max-width: 400px) {
  #about img,
  #home img {
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
    height: 200px;
  }
  #about {
    /* width: 20px; */
    word-wrap: break-word;
    word-break: break-all;
  }
}
</style>
