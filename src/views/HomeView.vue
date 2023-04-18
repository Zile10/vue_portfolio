<template>
  <div id="home">
    <div class="section-overlay">
        <h1 class="d-block intro animate__animated animate__bounceIn" data-aos="zoom-in">Hi There</h1>
        <div class="d-block">
          <h4 data-aos="fade-left">I am John-Bruce Noad. Welcome to my page!</h4>
          <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" class="profile-img img-fluid">
          <h5><strong>Intern Software & Web Developer</strong></h5>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  components: {
    
  }
}
</script>

<style scoped>
  #home {
    background-image: url(https://i.postimg.cc/7LdGmFry/lauren-mancke-unsplash-white-desk.jpg);
  }
  #home .profile-img {
    width: 350px;
    height: 350px;
    object-fit: cover;
    object-position: top;
    border-radius: 500px;
  }
  .profile-img {
    border-radius: 10px;
    box-shadow: 0 0 15px black;
    margin: 0 5px;
  }

  h1, h2, h3, h4, h5, h6, p{
    word-wrap: break-word;
  }
@media only screen and (max-width: 720px) {
  #home .profile-img {
    width: 300px;
    height: 300px;
  }

  #about {
    padding-bottom: 40px;
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
}
</style>