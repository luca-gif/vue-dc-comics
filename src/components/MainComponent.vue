<template>
  <main>
    <div class="container">
      ----> Content Goes Here!
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainComponent'
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
  height: 100px;
}

</style>