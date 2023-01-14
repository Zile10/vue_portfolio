<template>
  <div class="symbol">1</div>
  <div class="symbol">2</div>
  <div class="symbol">3</div>
  <div class="symbol">4</div>

  <div class="symbol">5</div>
  <div class="symbol">6</div>
  <div class="symbol">7</div>
  <div class="symbol">8</div>

  <div class="symbol">9</div>
  <div class="symbol">0</div>
  <div class="symbol">+</div>
  <div class="symbol">-</div>

  <div class="symbol">×</div>
  <div class="symbol">÷</div>
  <div class="symbol">√</div>
  <div class="symbol">=</div>
</template>
<script>
export default {
  
}
</script>
<style>
    div.symbol {
    width: 60px;
    height: 60px;
    position: absolute;
    left: 400px;
    top: 400px;
    animation: 4s infinite;
    font-size: 50px;
    font-weight: bold;
    /* text-shadow: 0 0 20px black, 0 0 15px white; */
  }
  div.symbol:nth-child(2) {
    top: 56%;
    left: 25%;
    animation: animateBubbles 6s alternate linear infinite;
    color: #32e7e4;
  }
  div.symbol:nth-child(3) {
    top: 40%;
    left: 73%;
    animation: animateBubbles 10s alternate linear infinite;
    color: #3e32e7;
  }
  div.symbol:nth-child(4) {
    top: 60%;
    left: 68%;
    animation: animateBubbles 4s alternate linear infinite;
    color: #b732e7;
  }

  div.symbol:nth-child(5) {
    top: 70%;
    left: 16%;
    animation: animateBubbles 5s alternate linear infinite;
    color: #e732c0;
  }
  div.symbol:nth-child(6) {
    top: 20%;
    left: 78%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #e73238;
  }
  div.symbol:nth-child(7) {
    top: 10%;
    left: 85%;
    animation: animateBubbles 10s alternate linear infinite;
    color: #32e7e4;
  }
  div.symbol:nth-child(8) {
    top: 19%;
    left: 13%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #3e32e7;
  }

  div.symbol:nth-child(9) {
    top: 65%;
    left: 80%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #e732c0;
  }
  div.symbol:nth-child(10) {
    top: 55%;
    left: 85%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #3e32e7;
  }
  div.symbol:nth-child(11) {
    top: 29%;
    left: 27%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #b732e7;
  }
  div.symbol:nth-child(12) {
    top: 2%;
    left: 12%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #32e7e4;
  }
  
  div.symbol:nth-child(13) {
    top: 10%;
    left: 20%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #e73238;
  }
  div.symbol:nth-child(14) {
    top: 40%;
    left: 80%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #3e32e7;
  }
  div.symbol:nth-child(15) {
    top: 34%;
    left: 22%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #b732e7;
  }
  div.symbol:nth-child(16) {
    top: 8%;
    left: 10%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #32e7e4;
  }
  
  div.symbol:nth-child(17) {
    top: 42%;
    left: 15%;
    animation: animateBubbles 9s alternate linear infinite;
    color: #e73238;
  }

  @keyframes animateBubbles {
    0% {
      transform: scale(1) translateY(0);
    }
    100% {
      transform: scale(1.5) translateY(100px) rotateY(360deg);
    }
  }

  @media only screen and (max-width: 1000px) {
    div.symbol {
      width: 45px;
      height: 45px;
    }
  }
  @media only screen and (max-width: 720px) {
    div.symbol {
      width: 40px;
      height: 40px;
    }
  }
  @media only screen and (max-width: 600px) {
    div.symbol {
      width: 35px;
      height: 35px;
    }
  }
  @media only screen and (max-width: 450px) {
    div.symbol {
      display: none;
    }
  }
</style>