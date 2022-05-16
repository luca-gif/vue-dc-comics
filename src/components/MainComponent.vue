<template>
  <main>
    <div class="container">    
 
      <CardComponent :fumetto="fumettoItem" v-for="(fumettoItem, index) in elencoFumetti" :key="index"/>

    </div>
  </main>
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


  .container{
    display: flex;
    flex-wrap: wrap;
  }
}

</style>