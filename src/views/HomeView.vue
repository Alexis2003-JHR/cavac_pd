<template>
  <div class="home">
    <video autoplay loop muted class="bg-video">
      <source src="../assets/Mountains.mp4" type="video/mp4">
    </video>

    <div class="home-text">
      <img src="@/assets/Logo.png" alt="">
      <div class="text-container">
        <div class="text-section">
          <h3>The travel like a breather for life.</h3>
          <p>Give me a moment, take a moment...</p>
        </div>
        <button>Look at destinations</button>
      </div>
    </div>

  </div>
</template>

<script>
export default{
  
}
</script>

<style lang="scss">
.home{
  position: relative;
}
.bg-video{
  width: 100%;
  max-width: 100%;
  max-height: 100vh;
  object-fit: cover;
}
.home-text{
  background-color: #000000da;
  display: flex;
  position: absolute;
  justify-content: center;
  align-items: center;
  width: 50%;
  height: 100vh;
  top: 0;
  img{
    position: absolute;
    top: 10%;
    left: 10%;
    width: 300px;
  }
}
.text-container{
  width: 80%;
  button{
    color: #EEEEEE;
    font-size: 30px;
    text-align: center;
    border: 3px solid #EEEEEE;
    background: none;
    padding: 10px 30px;
    transition: all 0.3s ease 0s;
  }
  button:hover{
    cursor: pointer;
    background-color: #eeeeee2f;
    box-shadow: 0px 15px 20px #eeeeee10;
    color: #fff;
  }
}
.text-section{
  color: #fff;
  margin-bottom: 60px;
  h3{
    font-size: 90px;
    font-weight: bold;
  }
  p{
    font-weight: 400;
    font-size: 35px;
  }
}
</style>