<template>
  <div id="resume">

    <EducationVue/>

    <SkillsVue/>

  </div>
</template>

<script>
// @ is an alias to /src
import EducationVue from '@/components/EducationVue.vue'
import SkillsVue from '@/components/SkillsVue.vue'

export default {
  name: 'HomeView',
  components: {
    EducationVue,
    SkillsVue,
  },
  data() {
    return {
      resume: [
        {
          //Education
          secondarySchool: '',
          qualification: '',
          year: '',
          additionalAchievements: '',
          courses: [],
        },
        {
          //Skills
        }
      ]
    }
  },
}
</script>

<style scoped>
  h1, h2, h3, h4, h5, h6, p{
    word-wrap: break-word;
  }
  #resume {
    background-image: url(https://i.postimg.cc/Dz84Q2Dg/georgie-cobbs-unsplash-white-wall-desk.jpg);
  }
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

  /* Education (End) */

  /* Skills */

  /* Skills (End) */


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