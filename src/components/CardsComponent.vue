<template>
  <div>
    <img :src="card.thumb" :alt="card.series">
    <p>{{card.series}}</p>
  </div>
</template>

<script>
export default {
  name: "CardsComponent",

  props:{
    card:Object
  }
}
</script>

<style lang="scss" scoped>

div{
  flex-basis: calc(100% /6);
  padding-top: 20px;
  img{
    width: 145px;
    height: 160px;
  }

  p{
    font-size: 15px;
    color: white;
  }
}

</style>