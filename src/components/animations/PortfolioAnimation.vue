<template>
  <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" loading="lazy" class="profile-img img-fluid">
  <img src="https://i.postimg.cc/FRXqRxkW/john-bruce-noad-portfolio-photo.png" alt="John-Bruce Profile" data-aos="fade-right" loading="lazy" class="profile-img img-fluid">
</template>
<script>
export default {
  
}
</script>
<style scoped>

.profile-img {
    width: 150px;
    height: 150px;
    object-fit: cover;
    object-position: top;
    border-radius: 500px;
    box-shadow: 0 0 15px black;
    margin: 0 5px;
  }
  img {
    position: absolute;
    animation: flip 8s linear infinite;
    top: 32%;
  }

  img:nth-child(2) {
    left: 73%;
  }
  img:nth-child(3) {
    left: 18%;
  }

  @keyframes flip {
    0% {
      transform: rotateY(0deg);
    }
    100% {
      transform: rotateY(360deg);
    }
  }
</style>