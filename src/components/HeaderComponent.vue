<template>
  <header>
    <div class="container">
      <div class="logo"><img src="../assets/img/dc-logo.png" alt="DC Logo"></div>
    <div class="menu">
      <ul v-for="(page, index) in pages" :key="`header ${index}`">
        <li><a @click="page.isActive = !page.isActive" :class="{'active' : page.isActive }" :href="page.url">{{page.name}}</a></li>
        <div :class="{'borderBottom' : page.isActive}"></div>
      </ul>
      
    </div>
    </div>
  </header>


</template>

<script>
export default {
  name: 'HeaderComponent',

  data(){
    return{

      pages: [
        {
          name: 'Characters',
          isActive: false,
          url: '#'
        },
        {
          name: 'Comics',
          isActive: false,
          url: '#'
        },
        {
          name: 'Movies',
          isActive: false,
          url: '#'
        },
        {
          name: 'Tv',
          isActive: false,
          url: '#'
        },
        {
          name: 'Games',
          isActive: false,
          url: '#'
        },
        {
          name: 'Collectibles',
          isActive: false,
          url: '#'
        },
        {
          name: 'Videos',
          isActive: false,
          url: '#'
        },
        {
          name: 'Fans',
          isActive: false,
          url: '#'
        },
        {
          name: 'News',
          isActive: false,
          url: '#'
        },
        {
          name: 'Shop',
          isActive: false,
          url: '#'
        },
      ]
    }
  },
  
}

</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

  .active{
    color: $primary-color;
  }

header{
  
  .container{
      display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;

  ul{
    list-style: none;
    padding-right: 10px;

    li{
      margin: 39px 0;
    }

    a{
      text-decoration: none;
      text-transform: uppercase;
      font-size: 13px;
    }

    .borderBottom{
      height: 4px;
      background-color: $primary-color;
      width: 90%;
      margin: 0 auto;
    }
  }

  .menu{
    display: flex;
  }
  
  img{
    width: 70%;
  }
  }
}


</style>