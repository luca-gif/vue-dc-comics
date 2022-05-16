<template>
  <div class="mini-wrapper">

      <div class="img-box">

      <img :src="fumetto.thumb" :alt="fumetto.type">

      </div>

      <div class="text">
      <h3>{{fumetto.series}}</h3>
      </div>
    
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
  width: 90%;
}

.img-box{
  height: 150px;
  overflow: hidden;
}

h3{
  font-size: 13px;
  padding: 20px 0;
}

.text{
  width: 90%;
}

</style>