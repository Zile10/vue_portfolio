<template>
  <div id="resume">

    <div id="education" class="d-flex flex-column align-items-center work-section">
      <div class="section-overlay">
        <h2 data-aos="zoom-in">Education</h2>
        <div data-aos="zoom-in" class="container education-block bevel">

          <h5 class="text-info">Secondary School:</h5>
          <p class="my-1"><strong class="text-primary">Wynberg Boys High School</strong></p>

          <h6 class="text-info">Qualification:</h6>
          <p class="my-1">National Senior Certificate</p>

          <h6 class="text-info">Year:</h6>
          <p class="my-1">2021</p>

          <h6 class="text-info">Additional Achievements:</h6>
          <p class="my-1">Chess Team</p>


          <hr data-aos="fade-right">
          <hr data-aos="fade-left">

          <h5 class="text-info">Courses:</h5>
          <p><strong class="text-primary">Bergvliet High - Continuing Edecation</strong></p>
          <p>- MS Excel Intermediate Course</p>
          <p>- MS Excel Advanced Course</p>

          <p><strong class="text-primary">Life Choices Academy</strong></p>
          <p>- 12 Month Coding Course</p>

        </div>
      </div>
    </div>

    <!-- Skills -->
    <div id="skills" class="d-flex flex-column align-items-center work-section">
      <div class="section-overlay">
        <h2 data-aos="zoom-in">Skills</h2>
        <div data-aos="zoom-in" class="d-flex flex-column align-items-center justify-content-center">

          <div class="container skills-block bevel mt-5">
            <h4 cla>Skills:</h4>
            <div class="container skills-grid">
              
              <div data-aos="fade-right" data-aos-duration="1000" class="html-skill w-100 d-flex flex-column align-items-center">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/color/48/null/html-5--v1.png"/>
                  HTML
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated bg-danger" role="progressbar" aria-label="Success example" style="width: 90%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100">
                    <strong>90% Proficiency</strong>
                  </div>
                </div>
              </div>
    
              <div data-aos="fade-left" data-aos-duration="1000" class="css-skill w-100 d-flex flex-column align-items-center">
                <img src="" alt="">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/color/48/null/css3.png"/>
                  CSS
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated bg-info" role="progressbar" aria-label="Info example" style="width: 90%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100">
                    <strong>90% Proficiency</strong>
                  </div>
                </div>
              </div>
    
              <div data-aos="fade-right" data-aos-duration="1000" class="javascript-skill w-100 d-flex flex-column align-items-center">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/color/48/null/javascript--v1.png"/>
                  JavaScript
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated bg-warning" role="progressbar" aria-label="Warning example" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">
                    <strong>80% Proficiency</strong>
                  </div>
                </div>
              </div>
    
              <div data-aos="fade-left" data-aos-duration="1000" class="bootstrap-skill w-100 d-flex flex-column align-items-center">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/color/48/null/bootstrap.png"/>
                  Bootstrap
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-label="Danger example" style="width: 85%" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100">
                    <strong>85% Proficiency</strong>
                  </div>
                </div>
              </div>

              <div data-aos="fade-right" data-aos-duration="1000" class="excel-skill w-100 d-flex flex-column align-items-center">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/color/48/null/ms-excel.png"/>
                  Excel
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated bg-success" role="progressbar" aria-label="Danger example" style="width: 65%" aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
                    <strong>65% Proficiency</strong>
                  </div>
                </div>
              </div>

              <div data-aos="fade-left" data-aos-duration="1000" class="soft-skills w-100 d-flex flex-column align-items-center">
                <h6 class="mb-0">
                  <img src="https://img.icons8.com/material-rounded/24/FFFFFF/group-task.png"/>
                  Soft-Skills
                </h6>
                <div class="progress">
                  <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-label="Danger example" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">
                    <strong>80% Proficiency</strong>
                  </div>
                </div>
              </div>

            </div>
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
  h1, h2, h3, h4, h5, h6, p{
    word-wrap: break-word;
  }
  #resume {
    background-image: url(https://i.postimg.cc/Dz84Q2Dg/georgie-cobbs-unsplash-white-wall-desk.jpg);
  }
  .section-overlay {
    width: 100%;
  }
  /* Education */
  .education-block {
    width: 70%;
    min-height: 400px;
    padding: 15px;
    background-color: var(--primaryColor);
    display: grid;
    grid-template-columns: 1fr 1fr;
  }

  .education-block p {
    grid-column: 2/-1;
  }
  .education-block h5, .education-block h6 {
    grid-column: 1/2;
  }
  .education-block h5 {
    text-decoration-line: underline;
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

  #skills strong {
    text-shadow: 2px 2px 4px black;
  }
  .progress {
    width: 90%;
    margin: 10px 0;
    background-color: #999
  }

  .skills-block {
    width: 70%;
    min-height: 400px;
    padding: 15px;
    background-color: var(--primaryColor);
  }

  .skills-block .container {
    margin-top: 20px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }

  .skills-block h4{
    margin: 15px;
  }


  .skills-block h6 {
    font-size: 15px;
    line-height: 20px;
  }
  .skills-block img {
    width: 20px;
  }
  .skills-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
  }

  .bootstrap-skill .progress-bar {
    background-color: blueviolet;
  }
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