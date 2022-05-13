<template>
  <section>
    <div class="container">

      <div class="item">
      <div class="item-logo">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>

      <div class="item-text">
        Digital Comics
      </div>
      </div>
      
      <div class="item">
      <div class="item-logo">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
      </div>

      <div class="item-text">
        DC Merchandise
      </div>
      </div>

      <div class="item">
      <div class="item-logo">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
      </div>

      <div class="item-text">
        Subscription
      </div>
      </div>

      <div class="item">
      <div class="item-logo">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
      </div>

      <div class="item-text">
        Comic Shop Locator
      </div>
      </div>

      <div class="item">
      <div class="item-logo">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
      </div>

      <div class="item-text">
        DC Power Visa
      </div>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionComponent'
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

  section{
    background-color: $primary-color;

    .container{
      @include center();
      height: 150px;
    
    .item{
      width: calc(100/5);
      display: flex;
      align-items: center;
      color: #fff;
      text-transform: uppercase;
      img{
        width: 40px;
        margin-right: 15px;
      }
    }
    }
  }

</style>