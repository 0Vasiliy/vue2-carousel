<template>
  <div id="app">
    <v-carousel-main/> 
  </div>
</template>

<script>
import vCarouselMain from './components/slider/v-Carousel-main.vue'
export default {
  name: 'App',
  components:{
    vCarouselMain,
  }
}
</script>

<style>
#app {
  font-family:Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
*{
    margin: 0 auto;
    padding: 0;      
}

html {
    box-sizing: border-box;
    height: 100%;
}

body{
    margin: 0;
    padding: 0;
    height: 100%;
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing: grayscale;
}
.container{
    margin: 0 auto;
    max-width: 1920px;
    width: 100%;
}
</style>
