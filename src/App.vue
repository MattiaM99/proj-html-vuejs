<template>
  <div>
    <Header/>
    <AboutAuthor/>
    <AudioBook/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import AboutAuthor from './components/AboutAuthor.vue'
import AudioBook from './components/AudioBook.vue'

export default {
  name: 'App',
  components: {
    Header,
    AboutAuthor,
    AudioBook
  }
}
</script>

<style lang="scss">
  @import './assets/style/generals.scss';
</style>
