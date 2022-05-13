<template>
  <div>
    <headerComponent/>
    <mainComponent/>
    <sectionComponent/>
    <footerComponents/>
</div>
</template>

<script>
import FooterComponents from './components/FooterComponents.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import SectionComponent from './components/SectionComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    SectionComponent,
    FooterComponents
    
  }
}
</script>

<style lang="scss">

  @import './assets/style/mixins';
  @import './assets/style/vars';
  @import './assets/style/global';
  @import './assets/style/utils';

</style>
