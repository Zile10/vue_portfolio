<template lang="">
  <div id="stars">
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>

    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>

    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>

  </div>
</template>
<script>
export default {
  
}
</script>
<style>
  div#stars {
    /* background-color: #333; */
    position: absolute;
    width: 90%;
    height: 100%;
    top: 0;
    left: 5%;
    z-index: 0;
    border-radius: 30px;
  }
  div.star {
    width: 10px;
    height: 10px;
    position: absolute;
    border-radius: 50px;
    animation: 4s linear infinite;
  }

  div.star:nth-child(2) {
    top: 56%;
    left: 25%;
    animation: twinkle 6s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #32e7e4;
    background-color: #32e7e4;
  }
  div.star:nth-child(3) {
    top: 40%;
    left: 73%;
    animation: twinkle 10s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #3e32e7;
    background-color: #3e32e7;
  }
  div.star:nth-child(4) {
    top: 50%;
    left: 88%;
    animation: twinkle 4s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #b732e7;
    background-color: #b732e7;
  }

  div.star:nth-child(5) {
    top: 72%;
    left: 15%;
    animation: twinkle 5s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #e732c0;
    background-color: #e732c0;
  }
  div.star:nth-child(6) {
    top: 20%;
    left: 78%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #e73238;
    background-color: #e73238;
  }
  div.star:nth-child(7) {
    top: 15%;
    left: 85%;
    animation: twinkle 10s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #32e7e4;
    background-color: #32e7e4;
  }
  div.star:nth-child(8) {
    top: 19%;
    left: 13%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #3e32e7;
    background-color: #3e32e7;
  }

  div.star:nth-child(9) {
    top: 65%;
    left: 80%;
    animation: twinkle 9s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #e732c0;
    background-color: #e732c0;
  }
  div.star:nth-child(10) {
    top: 69%;
    left: 87%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #3e32e7;
    background-color: #3e32e7;
  }
  div.star:nth-child(11) {
    top: 79%;
    left: 23%;
    animation: twinkle 9s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #b732e7;
    background-color: #b732e7;
  }
  div.star:nth-child(12) {
    top: 52%;
    left: 12%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #32e7e4;
    background-color: #32e7e4;
  }
  
  div.star:nth-child(13) {
    top: 10%;
    left: 20%;
    animation: twinkle 9s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #e73238;
    background-color: #e73238;
  }
  div.star:nth-child(14) {
    top: 25%;
    left: 25%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #3e32e7;
    background-color: #3e32e7;
  }
  div.star:nth-child(15) {
    top: 35%;
    left: 21%;
    animation: twinkle 9s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #b732e7;
    background-color: #b732e7;
  }
  div.star:nth-child(16) {
    top: 85%;
    left: 75%;
    animation: twinkle 9s alternate-reverse ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #32e7e4;
    background-color: #32e7e4;
  }
  
  div.star:nth-child(17) {
    top: 30%;
    left: 50%;
    animation: twinkle 9s alternate ease-in-out infinite;
    box-shadow: 0 0 30px 12px black, 0 0 15px 6px #fff, 0 0 5px 2px #e73238;
    background-color: #e73238;
  }

  @keyframes twinkle {
    0% {
      transform: scale(0.8) translateY(0px) translateX(0px);
      opacity: 0.3;
    }
    12.5% {
      transform: translateY(-5px) translateX(2px);
    }
    25% {
      transform: translateY(-2px) translateX(5px);
      opacity: 0.45;
    }
    37.5% {
      transform: translateY(2px) translateX(5px);
    }
    50% {
      transform: scale(1.2) translateY(5px) translateX(2px);
      opacity: 0.6;
    }
    62.5% {
      transform:translateY(5px) translateX(-2px);
    }
    75% {
      transform: translateY(2px) translateX(-5px);
      opacity: 0.75;
    }
    87.5% {
      transform: translateY(-2px) translateX(-5px);
    }
    100% {
      transform: scale(1.6) translateY(-5px) translateX(-2px);
      opacity: 0.9;
    }
  }

  /* @media only screen and (max-width: 1000px) {
    div.bubble {
      width: 45px;
      height: 45px;
    }
  }
  @media only screen and (max-width: 720px) {
    div.bubble {
      width: 40px;
      height: 40px;
    }
  }
  @media only screen and (max-width: 600px) {
    div.bubble {
      width: 35px;
      height: 35px;
    }
  }
  @media only screen and (max-width: 450px) {
    div.bubble {
      display: none;
    }
  } */

</style>