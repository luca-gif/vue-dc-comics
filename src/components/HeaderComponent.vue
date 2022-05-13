<template>
  <header>
    <div class="container">
      <div class="logo"><img src="../assets/img/dc-logo.png" alt=""></div>
    <div class="menu">
      <ul>
        <li><a href="#">HOME</a></li>
      </ul>
    </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

header{
  .container{
      display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  ul{
    list-style: none;
    a{
      text-decoration: none;
      color: black
    }
  }
  
  img{
    width: 70%;
  }
  }
}


</style>