<template>
  <div class="container-fluid articles-container">
    <div class="container articles-main">
      <div class="articles-title d-flex justify-content-between align-items-end">
        <div class="title-left">
          <h2>Recent Articles</h2>
          <h3>READ THE LATEST ENTRIES</h3>
        </div>
        <div class="title-right ">
          <button>All Articles</button>
        </div>
      </div>
      <div class="articles-main d-flex justify-content-between">
        <div class="articles-main-l text-center">
          <img src="../assets/img/20-Tips-600x353.jpg" alt="">
          <div class="articles-main-capt-l text-start">
            <h2>20 Creativity Tips</h2>
            <h4>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem, eum!</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Maiores, corporis laborum. Ducimus expedita minima magni sint enim fugiat, aliquam, nemo eaque veniam porro deserunt, quia eligendi id maxime possimus et.</p>
          </div>
        </div>
        <div class="articles-main-r">
          <div v-for="(article, index) in articles" :key="index" class="box p-3 bg-white text-center">
            <div class="img-box"><img :src="article.img" :alt="article.alt"></div>
            <div class="box-capt text-start">
              <h5>{{article.title}}</h5>
              <h6>{{article.date}} | {{article.comments}}</h6>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import image1 from "../assets/img/thumb-13-2x-320x202.jpg"
import image2 from "../assets/img/thumb-08-2x-320x202.jpg"

export default {
  name:"Articles",

  data(){
    return{
      articles:[
        {
          img: image1,
          alt: "image",
          title: "What's on your booklist?",
          date: "October 24th, 2019",
          comments: 0
        },  
        {
          img: image2,
          alt: "image",
          title: "Istanbul Travel Guide",
          date: "October 24th, 2019",
          comments: 0
        } 
      ]

    }
  }
}
</script>

<style lang="scss" scoped>
  .articles-container{
    background-color: #FEF7E9;
    .articles-main{
      padding: 100px 0;
      .articles-title{
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
        }
      }
      .articles-main-l{
        padding: 40px;
        max-width: 700px;
        min-height: 600px;
        background-color: #fff;
        img{
          margin-bottom: 25px;
        }
        h4{
          color: gray;
          font-size: 18px;
        }
      }
    }
  }
</style>