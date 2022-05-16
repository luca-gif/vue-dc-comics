<template>
  <div class="mini-wrapper">

      <div class="img-box">

      <img :src="fumetto.thumb" :alt="fumetto.type">

      </div>

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

.mini-wrapper{
  width: calc(100% / 6);
}

img{
  width: 150px;
}

.img-box{
  height: 150px;
  overflow: hidden;
  padding: 0px;
}

h3{
  font-size: 13px;
  padding: 20px 0;
}




</style>