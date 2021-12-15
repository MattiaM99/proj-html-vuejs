<template>
  <div class="footer-container container-fluid d-flex justify-content-center flex-column">
    <div class="footer-main d-flex justify-content-between align-items-center flex-row">
      <div class="row">
        <div class="col">
          <img src="../assets/img/author-logo-round-200x205.png" alt="">
        </div>
        <div class="col">
          <h3>ABOUT ME</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus odit corporis ut esse aspernatur maxime nam architecto, consequuntur rerum nostrum tenetur ipsum eligendi iusto expedita sit nesciunt pariatur provident magnam.</p>
        </div>
        <div class="col">
          <ul>
            <h3>USEFUL LINKS</h3>
            <li>
              <span> &#8250; </span> <a href="">Lorem, ipsum dolor.</a> 
            </li>         
            <li>
              <span> &#8250; </span> <a href="">Lorem, ipsum dolor.</a> 
            </li>         
            <li>
              <span> &#8250; </span> <a href="">Lorem, ipsum dolor.</a> 
            </li>         
            <li>
              <span> &#8250; </span> <a href="">Lorem, ipsum dolor.</a> 
            </li>         
            <li>
              <span> &#8250; </span> <a href="">Lorem, ipsum dolor.</a> 
            </li>         
          </ul>
        </div>
        <div class="col">
          <ul>
            <h3>CONTACT INFO</h3>
            <li>
              Lorem ipsum, dolor
            </li>               
            <li>
              Lorem ipsum, dolor
            </li>               
            <li>
              Lorem ipsum, dolor
            </li>               
            <li>
              <a href="">Lorem ipsum, dolor</a> 
            </li>
            <li>

            </li>               
          </ul>
        </div>
      </div>
    </div>
    <div class="container footer-bottom text-center">
      <p>&copy; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by Boolean</p>
    </div>
  </div>
</template>
<script>

export default {
  name:"Footer"
}
</script>

<style lang="scss" scoped>
  .footer-container{
    min-height: 500px;
    background-image: url("../assets/img/footer-3.jpg");
    background-size: cover;
    .footer-main{
      color: white;
      width: 100%;
      ul{
        list-style: none;
        span{
          font-size: 25px;
          font-weight: bold;
        }
        a{
          text-decoration: none;
          color: white;
        }
      }
    }
    .footer-bottom{
      color: white;
      padding-top: 100px;
    }
  }
</style>