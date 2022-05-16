<template>
  <div>
      <img :src="slide.image" :alt="slide.title">
      <h2>{{slide.title}}</h2>
      <span>{{slide.text}}</span>
  </div>
</template>

<script>
export default {
    name: "CardComp",
    props:{
        slide:Object,
    }

}
</script>

<style>

</style>