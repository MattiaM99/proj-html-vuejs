<template>
  <div class="audio-book">
    <div class="audio-book-top">
      <div class="audio-apps container d-flex justify-content-center align-items-center">
        <img src="../assets/img/ebay-logotan-2x-200x66.png" alt="">
        <img src="../assets/img/audible-logotan-2x-200x66.png" alt="">
        <img src="../assets/img/bb-logotan-2x-200x66.png" alt="">
        <img src="../assets/img/kindlefire-logotan-2x-200x66.png" alt="">
      </div>
    </div>
    <div class="audio-book-main container-fluid d-flex justify-content-center align-items-center">
      <div class="audio-img">
        <img src="../assets/img/audible-app-2x-400x418.png" alt="">
      </div>
      <div class="audio-description text-center ml-5">
        <h2>New AudioBook</h2>
        <h4>no time to read? no problem, listen to it.</h4>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem quo officiis exercitationem similique consequuntur consequatur modi distinctio, doloremque quaerat numquam?</p>
        <img src="../assets/img/audible-logo.png" alt="">
        <img src="../assets/img/bn-logo-tall.png" alt="">
        <img src="../assets/img/kindle-logo-tall.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"AudioBook"
}
</script>

<style lang="scss" scoped>
.audio-book{
  min-height: 500px;
  .audio-book-top{
    background-color: #FEF7E9;
    .audio-apps{
      padding: 50px 0;
      img{
        margin: 0 25px;
        cursor: pointer;
      }
    }
  }
  .audio-book-main{
    padding-top: 200px;
    background-image: url("../assets/img/banner.jpg");
    background-size: cover;
    .audio-description{
      width: 35%;
    h2{
      color: white;
      font-size: 50px;
    }
    h4{
      text-transform: uppercase;
      color: #FA991E;
    }
    p{
      font-size: 20px;
      color: #A39D95;
    }
    img{
      margin: 0 15px;
    }
    }
  }
}
</style>
  
