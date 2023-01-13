<template>
  <div class="home">
    <video autoplay loop muted class="bg-video">
      <source src="../assets/Mountains.mp4" type="video/mp4">
    </video>
  </div>
</template>

<script>
export default{
  
}
</script>

<style lang="scss">
.bg-video{
  width: 100%;
  max-width: 100%;
  max-height: 100vh;
  object-fit: fill;
  z-index: -100;
}
</style>