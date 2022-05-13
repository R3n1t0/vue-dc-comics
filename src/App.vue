<template>
  <div id="app">

    <HeaderComponent />
    <MainComponent />
    <MidleComponent />
    <FooterComponent />
    
  </div>
</template>

<script>

import HeaderComponent from "./components/HeaderComponent.vue"
import MainComponent from "./components/MainComponent.vue"
import MidleComponent from "./components/MidleComponent.vue"
import FooterComponent from "./components/FooterComponent.vue"

export default {
  name: 'App',

  components: {

      HeaderComponent, 
      MainComponent, 
      MidleComponent, 
      FooterComponent 
  }
}
</script>

<style lang="scss">
@import url(./assets/style/_general.scss);
@import url(./assets/style/_utils.scss);
@import url(./assets/style/_vars.scss);
</style>
