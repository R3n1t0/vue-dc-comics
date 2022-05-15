<template>
  <div id="app">

    <HeaderComponent />
    <MainComponent />
    <MidleComponent />
    <FooterComponent />
    <BottomComponent />
    
  </div>
</template>

<script>

import HeaderComponent from "./components/HeaderComponent.vue"
import MainComponent from "./components/MainComponent.vue"
import MidleComponent from "./components/MidleComponent.vue"
import FooterComponent from "./components/FooterComponent.vue"
import BottomComponent from "./components/BottomComponent.vue"

export default {
  name: 'App',

  components: {
    HeaderComponent, 
    MainComponent, 
    MidleComponent, 
    FooterComponent,
    BottomComponent
  }
}
</script>

<style lang="scss">

@import "./assets/style/_general.scss";
@import "./assets/style/_utils.scss";
@import "./assets/style/_vars.scss";
@import "./assets/style/_mixin.scss";

</style>
