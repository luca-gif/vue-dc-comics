<template>
<div>

  <div class="jumbotron"></div>

  <main>
    
    <div class="btn-current">CURRENT SERIES</div>

    <div class="container">    
 
      <CardComponent :fumetto="fumettoItem" v-for="(fumettoItem, index) in elencoFumetti" :key="index"/>

      <div class="btn-load">LOAD MORE</div>
    </div>

  </main>
  </div>
</template>

<script>
import CardComponent from "./CardComponent.vue";
export default {

  name: 'MainComponent',
  components: {
    CardComponent
  },
  props: {
    elencoFumetti: Object
  },

}
</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

main{
  @include center();
  background-color: black;
  color: #fff;
  padding: 40px 0;
  position: relative;

  .container{
    display: flex;
    flex-wrap: wrap;
  }
}

  .jumbotron{
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
  }

  .btn-current{
    position: absolute;
    top:-20px;
    left: 250px;
    background-color: $primary-color;
    font-size: 18px;
    font-weight: bolder;
    padding: 10px;
  }

  .btn-load{
    background-color: $primary-color;
    font-weight: bolder;
    padding: 10px 40px;
    margin: 0 auto;
  }


</style>