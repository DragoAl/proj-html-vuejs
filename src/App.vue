<template>
  <div id="app">
    <MyHeader
    :menuElements = 'menuItems'
    />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
  },

  data() {
    return {
     menuItems: [
      {
        icon: "fab fa-pagelines",
        title: 'TREATMENTS',
        subtitle: 'Face & Body'
        
      },
      
      {
        icon: "fas fa-male",
        title: 'ABOUT',
        subtitle: 'Our Team'
        
      },
      
      {
        icon: "fas fa-heart",
        title: 'JOURNAL',
        subtitle: 'Tips & Tricks'
        
      },
      
      {
        icon: "fas fa-bookmark",
        title: 'BOOK NOW',
        subtitle: 'Special Offers'
        
      },
     ] 


    }
  }
}
</script>

<style lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
