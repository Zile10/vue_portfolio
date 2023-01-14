<template>
  <!-- <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
 -->
  <div class="img"></div>
  <div class="img"></div>
  <div class="img"></div>
  <div class="img"></div>
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
  }
  div{
    position: absolute;
    width: 150px;
    border-radius: 100%;
    height: 150px;
    background-color: #fff;
    top: 10%;
    animation: spinFall 8s linear infinite;;
  }

  .img:nth-child(2) {
    left: 24%;
  }
  .img:nth-child(3) {
    left: 11%;
  }
  .img:nth-child(4) {
    left: 65%;
  }
  .img:nth-child(5) {
    left: 78%;
  }

  @keyframes spinFall {
    0% {
      transform: rotateY(0deg) translateY(0px);
      opacity: 0;
    }
    20% {
      opacity: 1;
    }
    80% {
      opacity: 1;
    }
    100% {
      transform: rotateY(360deg) translateY(300px);
      opacity: 0;
    }
  }

</style>