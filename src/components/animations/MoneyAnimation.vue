<template>
  
  <div class="div-1">$</div>
  <div class="div-2">$</div>
  <div class="div-1">$</div>
  
  <div class="div-2">$</div>
  <div class="div-1">$</div>
  <div class="div-2">$</div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
  div {
    width: 60px;
    height: 60px;
    position: absolute;
    top: 40%;
    font-weight: bolder;
    font-size: xx-large;
    text-shadow: 1px 1px 0 white, -1px 1px 0 white, 1px -1px 0 white, -1px -1px 0 white;
  }
  div.div-1 {
    color: #42b983;
    animation: 1s animateMoney1 alternate linear infinite;
  }
  div.div-2 {
    color: #6bff2c;
    animation: 1s animateMoney2 alternate linear infinite;
  }

  div:nth-child(2) {
    left: 10%;
  }
  div:nth-child(3) {
    left: 18%;
  }
  div:nth-child(4) {
    left: 26%;
  }

  div:nth-child(5) {
    left: 70%;
  }
  div:nth-child(6) {
    left: 78%;
  }
  div:nth-child(7) {
    left: 86%;
  }

  @keyframes animateMoney1 {
    0% {
      scale: 2;
      color: #42b983;
    }
    100% {
      scale: 2.5;
      color: #6bff2c;
    }
  }
  @keyframes animateMoney2 {
    0% {
      scale: 2;
      color: #6bff2c;
    }
    100% {
      scale: 2.5;
      color: #42b983;
    }
  }

  @media only screen and (max-width: 450px) {
    div {
      display: none;
    }
  }
</style>