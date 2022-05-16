<template>
  <div>

      <img :src="fumetto.thumb" :alt="fumetto.type">

      <h3>{{fumetto.series}}</h3>
    
  </div>
</template>

<script>

//import fumetti from '../assets/data/dc-comics.json'

export default {
  name: 'CardComponent',

   props: {
     fumetto: Object
   },

}
</script>-

<style lang="scss" scoped>

div{
  width: calc(100% / 6);
}



</style>