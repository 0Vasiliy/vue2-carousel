<template>
    <section class="v-carousel-main  col-xl-9 col-md-9 col-10">      
      <div class="container">
        <v-carousel
                :carousel_data="sliderItems"
                :interval="2000"
          />
          <v-carousel-item/>
      </div>
  </section>
</template>

<script>
import vCarousel from './v-Carousel.vue';
import vCarouselItem from './v-Carousel-item.vue';

export default {
    name: 'vCarouselMain',
    components: {
    vCarousel,
    vCarouselItem
  },
  data(){
    return{
      sliderItems:[
        {id:1, name: 'img1', img:'1.jpg'},
        {id:2, name: 'img2', img:'2.jpg'},
        {id:3, name: 'img3', img:'3.jpg'},
        {id:4, name: 'img4', img:'4.jpg'},
        {id:5, name: 'img5', img:'5.jpg'},
      ]
    }
  }
}

</script>
<style scoped>

  .v-carousel-main{
    max-width: 1400px;
    display: flex;
    align-items: center;
    background: hsla(186, 33%, 94%, 1);
    background: linear-gradient(90deg, hsla(186, 33%, 94%, 1) 0%, hsla(216, 41%, 79%, 1) 100%);    
    background: -moz-linear-gradient(90deg, hsla(186, 33%, 94%, 1) 0%, hsla(216, 41%, 79%, 1) 100%);   
    background: -webkit-linear-gradient(90deg, hsla(186, 33%, 94%, 1) 0%, hsla(216, 41%, 79%, 1) 100%);   
    filter: gradient( startColorstr="#EBF4F5", endColorstr="#B5C6E0", GradientType=1 );
    margin-top: 30px;
    border-radius: 20px;
    background-size: auto 100%;
  }


</style>