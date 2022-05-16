<template>
  <main>
    <div class="jumbotron"></div>
    <CardsComponent
      
    />
    
  </main>
</template>

<script>
/* import comicsCards from "../assets/data/comicsCards" */
import CardsComponent from "../components/CardsComponent.vue"

export default {
  name: "MainComponent",

  components: {
    CardsComponent
  }
}
</script>

<style lang="scss" scoped>

main{
  background-color: #1c1c1c;

  .jumbotron{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
  }
}
</style>