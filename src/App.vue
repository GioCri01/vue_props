<template>
  <div id="app">
   <CardComp
   v-for="(slideItem,index) in sliderImages" :key="`slide-${index}`"
   :slide="slideItem"
   
   />
   <CardDueComp
   v-for="(slideItem,index) in sliderImages" :key="`slideDue-${index}`"
   :cardimage="slideItem.image"
   :cardtitle="slideItem.title"
   :carddescription="slideItem.text"
   
   />
  </div>
</template>

<script>
import sliderImages from './assets/data/sliderImages'
import CardComp from './components/CardComp.vue'
import CardDueComp from './components/CardDueComp.vue'
export default {
 
  name: 'App',
  components: {
    CardComp,
    CardDueComp,
},
  data(){
    return{
      sliderImages
    }
  },
  mounted(){
    console.log(this.sliderImages);
  }
  
}
</script>

<style>

</style>
