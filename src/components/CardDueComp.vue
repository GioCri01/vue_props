<template>
  <div>
      <img :src="cardimage" :alt="cardtitle">
      <h2>{{cardtitle}}</h2>
      <span>{{carddescription}}</span>
  </div>
</template>

<script>
export default {
    name: "CardDueComp",
    props:{
        cardimage:String,
        cardtitle:String,
        carddescription:String

    }

}
</script>

<style>

</style>