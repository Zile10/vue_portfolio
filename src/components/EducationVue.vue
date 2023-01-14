<template>
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
</template>
<script>
export default {
  
}
</script>
<style scoped>
  * {
    word-wrap: break-word;
    word-break: break-all;
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
    border-radius: 3px;
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