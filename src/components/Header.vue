<template>
  <div class="container-fluid header">
    <nav class="navbar navbar-expand-lg static-top header-top justify-content-between">
      <div class="logo">
        <img src="../assets/img/author-logo-round-small.png" alt="">
      </div>
      <div class="navbar-collapse">
        <ul class="navbar-nav ms-auto">
            <li v-for="(link, index) in links" 
            :key="index" 
            :class="{active : (index === counter)}" class="nav-item">
              <a class="nav-link mx-1 px-3" href="#">{{link.name}}</a>
            </li>  
          </ul>
      </div>
    </nav>
    <div class="header-central container-fluid d-flex justify-content-between">
      <div class="row">
        <div class="header-central-l col d-flex align-items-center">
          <div class="caption">
            <h1>Damon Vaughn</h1>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsa vel quaerat expedita eos voluptatibus natus!</p>
            <span>-The New York Times</span>
          </div>
        </div>    
      </div>
      <div class="header-central-r col">
        <div class="header-central-rtop d-flex justify-content-end">
          <ul>
            <li><p>Demos</p></li>
            <li>
              <span>$39</span>
              <p>On Sale</p>
            </li>
          </ul>
        </div>
        <div class="header-central-rbottom">
          <div class="d-flex justify-content-around">
            <div class="book-img">
              <img src="../assets/img/book-widget.png" alt="">
            </div>
            <div class="book-description">
              <h2>Latest Book Release</h2>
              <h5>d. vaughn autobiography</h5>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis sed fugiat molestias est, cum recusandae expedita enim rerum nemo reiciendis?</p>
            </div>
          </div>
          <div class="buttons d-flex justify-content-center align-items-center">
            <button class="amazon-btn shadow p-3 my-1 bg-body rounded">Buy on Amazon</button>
            <button class="apple-btn shadow p-3 my-1 bg-body rounded">Buy on AppStore</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: "Header",

  data(){
    return{
      links:[
        {
          url: "/home",
          name: "Home",
          active: false,
        },
        {
          url: "/Aboutme",
          name: "About Me",
          active: false,
        },
        {
          url: "/testimonials",
          name: "testimonials",
          active: false,
        },
        {
          url: "/myblog",
          name: "My blog",
          active: false,
        },
        {
          url: "/meetups",
          name: "Meetups",
          active: false,
        },
        {
          url: "/shop",
          name: "Shop",
          active: false,
        },
        {
          url: "/contactme",
          name: "Contact Me",
          active: false,
        },
        {
          url: "/cart",
          name: "Cart",
          active: false,
        }
      ],
      counter: 0,
    }
  }
}
</script>

<style scoped lang="scss">
  .container-fluid{
    padding-right: 0!important;
  }
  .header{
    background-image: url('../assets/img/footer-3.jpg');
    background-size: cover;
    height: 800px;
  }
  .header-top{
    height: 15%;
    position: relative;
  }
  a{
    color: white !important;
  }
  .logo{
    position: absolute;
    top: 10px;
    left: 80px;
  }
  .nav-link{
    font-weight: bold;
  }
  .active{
    color: #F5C358 !important;
    border-top: 3px solid #F5C358
  }
  .header-central{
    margin-top: 80px;
    .header-central-l{
     margin-left: 200px;
     .caption{
       h1{
       color:#F5C358
      }
      p{
       color: white;
       font-size: 45px;
      }
      span{
        font-size: 25px;
        color: #A39D95;
        font-style: italic;
      }
     }
    }
    .header-central-r{
      width: 45%;
      height: 100%;
      .header-central-rtop{
        margin-right: 25px;
        ul{
          list-style: none;
          li{
            text-align: center;
            height: 80px;
            width: 80px;
            margin-bottom: 25px;
            background-color: white;
            border-radius: 10px;
            cursor: pointer;
          }
          span{
            color: #60BA77;
            font-size: 25px;
          }
        }
      }
      .header-central-rbottom{
        background-color: white;
        padding: 25px;
        .book-description{
          width: 35%;
          h5{
            color: #F6C353;
            text-transform: uppercase;
          }
        }
        .buttons{
          height: 80px;
          button{
            width: 300px;
            border: 1px solid grey;
            background-color: #fff;
            &:hover{
              border: 2px solid #3DD291;
              transition: 0.1s;
            }
          }
          .amazon-btn{
            border-radius: 5px 0 0 5px !important;
          }
          .apple-btn{
            border-radius: 0 5px 5px 0 !important;
          }
        }
      }
    }
  }
</style>