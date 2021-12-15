<template>
  <div class="container bio-container">
    <div class="bio-title text-center d-flex justify-content-center align-items-center flex-column">
      <h2>Dig A Little Deeper Into Damon Vaughn</h2>
      <h5>find out more about the author himself</h5>
    </div>
    <div class="bio-main d-flex justify-content-between align-items-center text-center">
      <div v-for="(item, index) in items" :key="index" class="box">
        <img :src="item.img" :alt="item.alt">
        <div class="box-caption text-center">
          <h3>{{item.title}}</h3>
          <p>{{item.caption}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import image1 from "../assets/img/box-1.jpg"
import image2 from "../assets/img/box-3.jpg"
import image3 from "../assets/img/box-4.jpg"
export default {
  name:"Authorbio",
  data(){
    return{
      items:[
        {
          img: image1,
          alt:"about me",
          title:"About Me",
          caption:"lorem ipsum"
        },
        {
          img: image2,
          alt:"Latest books",
          title:"My Latest Books",
          caption:"lorem ipsum"
        },
        {
          img: image3,
          alt:"Book Signing",
          title:"Book Signing",
          caption:"lorem ipsum"
        }
      ]
    }
  }

}
</script>

<style lang="scss" scoped>
  .bio-container{
    padding: 50px 0;
    .bio-title{
      h5{
        color: gray;
        text-transform: uppercase;
        font-size: 15px;
      }
    }
    .bio-main{
      padding-top: 50px;
      .box{
        position: relative;
        height: 400px;
        width: 400px;
        opacity: 0.9;
        img{
          background-size: cover;
          height: 100%;
          width: 100%;
          border-radius: 0 0 50px 0;
          filter: brightness(40%);
          cursor: pointer;
        }
        .box-caption{
          position: absolute;
          z-index: 9;
          bottom: 0;
          width: 100%;
          h3{
            color: white;
          }
          p{
            color: #F4B429;
          }
        }
      }
    }
  }
</style>