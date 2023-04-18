<template>
  <img src="https://i.postimg.cc/Yq9hkTMv/planet-remix-fixed.webp" alt="">
  <img src="https://i.postimg.cc/Yq9hkTMv/planet-remix-fixed.webp" alt="">
</template>
<script>
export default {
  
}
</script>
<style scoped>
  img {
    position: absolute;
    width: 150px;
    border-radius: 100%;
    animation: 4s 1s linear infinite alternate float;
    top: 30%;
  }
  img:nth-child(2) {
    left: 20%;
  }
  img:nth-child(3) {
    left: 72%;
  }

  @keyframes float {
    0% {
      transform: translateY(15px);
    }
    25% {
      transform: translateY(4px);
    }
    50% {
      transform: translateY(-13px);
    }
    75% {
      transform: translateY(-29px);
    }
    100% {
      transform: translateY(-40px);
    }
  }

  @media only screen and (max-width: 1000px) {
    img {
      scale: 0.9;
    }

    img:nth-child(2) {
      left: 21%;
    }
    img:nth-child(3) {
      left: 8%;
    }
    img:nth-child(4) {
      left: 61%;
    }
    img:nth-child(5) {
      left: 75%;
    }

  }
  @media only screen and (max-width: 720px) {
    img {
      scale: 0.75;
    }
  }
  @media only screen and (max-width: 600px) {
    img {
      scale: 0.6;
    }
    img:nth-child(2) {
      left: 16%;
    }
    img:nth-child(3) {
      left: 3%;
    }
    img:nth-child(4) {
      left: 56%;
    }
    img:nth-child(5) {
      left: 70%;
    }
  }
  @media only screen and (max-width: 500px) {
    img {
      display: none;
    }
  }

</style>