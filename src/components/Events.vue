<template>
  <div class="container-fluid events-container d-flex justify-content-center align-items-center flex-column">
    <h2>Upcoming Events</h2>
    <h3>meet the author in person</h3>
    <div class="container upcoming-events d-flex  justify-content-between align-items-center ">
      <ul class="d-flex flex-row">
        <li v-for="(event, index) in events" :key="index" class="event text-center">
          <div class="img-box">
            <img :src="event.img" :alt="event.alt">
          </div>
          <h4 class="event-name">{{event.title}}</h4>
          <p>{{event.description}}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name:"Events",

  data(){
    return{
      events:[
        {
          img: "img/event-05-400x240.jpg",
          alt: "image",
          title: "Chicago Book Signing",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis magnam, tempora ut optio porro voluptatum vel quibusdam, modi maxime necessitatibus earum? Distinctio, officia? Velit neque aliquid atque, voluptatibus corporis earum.",
        },  
        {
          img: "img/event-04-400x240.jpg",
          alt: "image",
          title: "Meet & Greet With Amanda",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis magnam, tempora ut optio porro voluptatum vel quibusdam, modi maxime necessitatibus earum? Distinctio, officia? Velit neque aliquid atque, voluptatibus corporis earum.",
        },  
        {
          img: "img/event-07-400x240.jpg",
          alt: "image",
          title: "Open Book: Dialogues",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis magnam, tempora ut optio porro voluptatum vel quibusdam, modi maxime necessitatibus earum? Distinctio, officia? Velit neque aliquid atque, voluptatibus corporis earum.",
        }  
      ]

    }
  }
}
</script>

<style lang="scss" scoped>
  .events-container{
    background-color: #FEF7E9;
    padding-top: 50px;
    h3{
      text-transform: uppercase;
      color: #F4B429;
      font-size: 15px;
    }
    .upcoming-events{
      ul{
        list-style: none;
        .event{
          min-height: 500px;
          background-color: #fff;
          margin: 0 50px;
          .event-name{
            border-bottom: 1px solid gray;
            padding: 25px;
            font-size: 20px;
          }
        }
      }
    }
  }
</style>