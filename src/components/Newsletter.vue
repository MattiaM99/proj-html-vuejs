<template>
  <div class="container-fluid newsletter-container d-flex text-center justify-content-center align-items-center flex-column ">
    <div class="container newsletter-main">
      <h2>Subscribe To My Newsletter</h2>
      <h4>be notified about signing tour dates</h4>
      <input type="text" placeholder="Insert Your Mail">
      <button>Subscribe</button>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum, labore?</p>
    </div>
  </div>
</template>

<script>
export default {
  name:"Newsletter"
}
</script>

<style lang="scss" scoped>
  .newsletter-container{
    background-image: url("../assets/img/banner-2.jpg");
    background-size: cover;
    min-height: 400px;
    opacity: 0.9;
    .newsletter-main{
      h2{
        color: white;
      }
      h4{
        color:#F4B429;
        text-transform: uppercase;
        font-size: 15px;
        margin: 25px 0;
      }
      input{
        padding: 10px 25px;
        border: 0;
        border-radius: 5px;
        margin: 20px 10px;
      }
      button{
        padding: 10px 35px;
        border: 0;
        border-radius: 5px;
        background-color: #49A987;
        color: white;
      }
      p{
        color: gray;
      }
    }
  }
</style>