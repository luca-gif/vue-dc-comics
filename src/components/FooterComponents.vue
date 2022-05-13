<template>
  <footer>
      <div class="footer-top">

        <div class="container">



        </div>
        
      </div>

      <div class="footer-bottom">

        <div class="container">
          
        </div>

      </div>

  </footer>
</template>

<script>
export default {
  name: 'FooterComponent'
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

  footer{
    .footer-top{
      height: 300px;
      background-image: url(../assets/img/footer-bg.jpg);
      display: flex;
      flex-direction: column;
    }
  }



</style>