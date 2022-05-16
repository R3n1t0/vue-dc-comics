<template>
  <main>
    <div class="jumbotron">
      <span>CURRENT SERIES</span>
    </div>

    <div class="container cards-container">
      <CardsComponent 
        v-for="(cardItem,index) in comicsCards" :key="`cards-${index}`"
        :card="cardItem"
      />
    </div>
    
    <button>LOAD MORE</button>
    
  </main>
</template>

<script>
import comicsCards from "../assets/data/comicsCards"
import CardsComponent from "../components/CardsComponent.vue"

export default {
  name: "MainComponent",

  components: {
    CardsComponent
  },

  data(){
    return{
      comicsCards
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/_vars.scss";
@import "../assets/style/_mixin.scss";

main{
  background-color: #1c1c1c;
  text-align: center;

  .jumbotron{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    position: relative;
    span{
      position: absolute;
      bottom: -15px;
      left: 230px;
      background-color: $primary-color;
      color: white;
      padding: 5px 30px;
      font-weight: bold;
    }
  }

  .cards-container{
    width: 70%;
    display: flex;
    flex-wrap: wrap;
    padding: 20px;
  }

  button{
    padding: 5px 30px;
    margin-bottom: 3rem;
    background-color: $primary-color;
    border: none;
    color: white;
    font-weight: bold;
  }
}
</style>