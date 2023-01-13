<template>
  <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
  <img src="https://picsum.photos/id/237/200/200" alt="">
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
  img:nth-child(2) {
    left: 24%;
  }
  img:nth-child(3) {
    left: 11%;
  }
  img:nth-child(4) {
    left: 65%;
  }
  img:nth-child(5) {
    left: 78%;
  }
</style>