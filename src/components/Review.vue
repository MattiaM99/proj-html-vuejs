<template>
  <div class="container review-container">
    <div class="review-title d-flex justify-content-between align-items-end">
      <div class="title-left">
        <h2>What the critics say</h2>
        <h3>TESTIMONIALS FROM AROUND THE WORLD</h3>
      </div>
      <div class="title-right ">
        <button>Read All Testimonials</button>
      </div>
    </div>
    <div class="review-main d-flex justify-content-between">
      <div class="review-main-l">
        <div class="rev-main-l-title text-center">
          <h4>Best Author Of His Generation</h4>
        </div>
        <div class="rev-main-l-desc">
          <h6>This book will change your perspective of life</h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus itaque obcaecati dolores neque nam iusto in tenetur. Itaque, assumenda!</p>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus itaque obcaecati dolores neque nam iusto in tenetur. Itaque, assumenda!</p>
        </div>
      </div>
      <div class="review-main-r">
        <ul>
          <li>
            <div class="box text-center">
              <h4>Lorem, ipsum dolor.</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis rem a placeat quis aut exercitationem quam aliquam numquam natus quidem, culpa quibusdam velit reiciendis voluptatum omnis cumque doloremque! Illo, vero!</p>
            </div>
            <div class="journal d-flex justify-content-start ">
              <img src="../assets/img/theguardian-xsmall.png" alt="">
              <p>Gerald Hendley, The Guardian</p>
            </div>
          </li>  
          <li>
            <div class="box text-center">
              <h4>Lorem, ipsum dolor.</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis rem a placeat quis aut exercitationem quam aliquam numquam natus quidem, culpa quibusdam velit reiciendis voluptatum omnis cumque doloremque! Illo, vero!</p>
            </div>
            <div class="journal d-flex justify-content-start ">
              <img src="../assets/img/globe-xsmall.png" alt="">
              <p>Mary Maxey, The Globe and Mail</p>
            </div>
          </li>  
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"Review"
}
</script>

<style lang="scss" scoped>
  .review-container{
    padding: 100px 0;
    h2{
      font-size: 45px;
    }
    h3{
      font-size: 20px;
      color: grey;
    }
    button{
      background-color: #F4B429;
      color: white;
      padding: 10px 25px;
      border: 0;
      border-radius: 5px;
      &:hover{
        background-color: #F4A700;
        transition: 0.8s;
      }
    }
    .review-main{
      margin-top: 80px;
      .review-main-l{
        min-height: 600px;
        width: 600px;
        border-radius: 0 0 50px 0;
        padding: 50px;
        background-image: url("../assets/img/testimonial2-2x.jpg");
        opacity: 0.9;
        background-size: cover;
        color: white;
        .rev-main-l-title{
          padding: 25px 0;
          margin-bottom: 25px ;
          border-bottom: 1px solid gray;
        }
        h6{
          font-size: 20px;
        }
      }
      .review-main-r{
        ul{
          list-style: none;
          li{
            margin-bottom: 100px;
            .box{
              position: relative;
              background-color: #FEF7E9;
              min-height: 200px;
              width: 500px;             
              padding: 20px;
            }
            .box::after{
              content: '';
              position: absolute;
              bottom: -10px;
              left: 0;
              width: 20px;
              height: 20px;
              background: linear-gradient(30deg, white 10px, transparent 0%), linear-gradient(0deg, #FEF7E9 10px, transparent 0%);
              background-size: 20px;
            }
            .journal{
              padding: 10px;
              img{
                width: 35px;
                height: 40px;
                margin-right: 10px;
              }
            }
          }
        }
      }
    }
  }
</style>