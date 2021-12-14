<template>
  <div id="app">
    <MyHeader
    :menuElements = 'menuItems'
    />
    <MyMain/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain
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
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
.btn {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  font-size: 14px;
  // width: 200px;
  padding: 5px 30px;
  border-radius: 20px;
  border: none;
  margin: 10px 0;
  font-weight: 1000;
  cursor: pointer;
}
.btn-colored {
  background-color:#d3cac0;
  color: white;
  
}
.btn-empty {
  background-color: transparent;
  border: 1px solid #bcafa1;
  color: #bcafa1;
  margin: 30px;
}
</style>
