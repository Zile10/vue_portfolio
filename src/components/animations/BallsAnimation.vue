<template lang="">
  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>

  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>

  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>

</template>
<script>
export default {
  
}
</script>
<style scoped>
  div.bubble {
    width: 60px;
    height: 60px;
    position: absolute;
    border: 2px solid white;
    border-radius: 50px;
    left: 400px;
    top: 400px;
    animation: 4s linear infinite;
  }
  div.bubble:nth-child(2) {
    top: 56%;
    left: 25%;
    animation: animateBubbles 6s linear infinite;
    border-color: #32e7e4;
    background-color: #32e7e44d;
  }
  div.bubble:nth-child(3) {
    top: 40%;
    left: 73%;
    animation: animateBubbles 5.5s linear infinite;
    border-color: #3e32e7;
    background-color: #3e32e74d;
  }
  div.bubble:nth-child(4) {
    top: 60%;
    left: 68%;
    animation: animateBubbles 4s linear infinite;
    border-color: #b732e7;
    background-color: #b732e74d;
  }

  div.bubble:nth-child(5) {
    top: 70%;
    left: 16%;
    animation: animateBubbles 5s linear infinite;
    border-color: #e732c0;
    background-color: #e732c04d;
  }
  div.bubble:nth-child(6) {
    top: 20%;
    left: 78%;
    animation: animateBubbles 9s linear infinite;
    border-color: #e73238;
    background-color: #e732384d;
  }
  div.bubble:nth-child(7) {
    top: 10%;
    left: 85%;
    animation: animateBubbles 9.8s linear infinite;
    border-color: #32e7e4;
    background-color: #32e7e44d;
  }
  div.bubble:nth-child(8) {
    top: 19%;
    left: 13%;
    animation: animateBubbles 9s linear infinite;
    border-color: #3e32e7;
    background-color: #3e32e74d;
  }

  div.bubble:nth-child(9) {
    top: 65%;
    left: 85%;
    animation: animateBubbles 7.5s linear infinite;
    border-color: #e732c0;
    background-color: #e732c04d;
  }
  div.bubble:nth-child(10) {
    top: 65%;
    left: 80%;
    animation: animateBubbles 8s linear infinite;
    border-color: #3e32e7;
    background-color: #3e32e74d;
  }
  div.bubble:nth-child(11) {
    top: 29%;
    left: 27%;
    animation: animateBubbles 8.5s linear infinite;
    border-color: #b732e7;
    background-color: #b732e74d;
  }
  div.bubble:nth-child(12) {
    top: 2%;
    left: 12%;
    animation: animateBubbles 6.5s linear infinite;
    border-color: #32e7e4;
    background-color: #32e7e44d;
  }
  
  div.bubble:nth-child(13) {
    top: 10%;
    left: 20%;
    animation: animateBubbles 10s linear infinite;
    border-color: #e73238;
    background-color: #e732384d;
  }

  @keyframes animateBubbles {
    0% {
      transform: scale(0.4) translateY(0);
    }
    100% {
      transform: scale(1.3) translateY(100px);
    }
  }

  @media only screen and (max-width: 1000px) {
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
  }

</style>