<template>
  <div>
    <Header/>
    <AboutAuthor/>
    <AudioBook/>
    <Review/>
    <Events/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import AboutAuthor from './components/AboutAuthor.vue'
import AudioBook from './components/AudioBook.vue'
import Review from './components/Review.vue'
import Events from './components/Events.vue'

export default {
  name: 'App',
  components: {
    Header,
    AboutAuthor,
    AudioBook,
    Review,
    Events
  }
}
</script>

<style lang="scss">
  @import './assets/style/generals.scss';
</style>
