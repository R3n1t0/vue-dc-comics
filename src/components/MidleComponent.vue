<template>
  <div class="container-fluid">
    <div class="container">
      <div v-for="(item, index) in digitalDc" :key="`menu-${index}`" class="digital-dc">
        <img :src="item.urlImage" alt="">
        <p>{{item.title}}</p>
      </div>
    </div>
  </div>

</template>

<script>
import uno from "../assets/img/buy-comics-digital-comics.png"
import due from "../assets/img/buy-comics-merchandise.png"
import tre from "../assets/img/buy-comics-subscriptions.png"
import quatro from "../assets/img/buy-comics-shop-locator.png"
import cinque from "../assets/img/buy-dc-power-visa.svg"


export default {
  name: "MidleComponent",

  data(){
    return{
      digitalDc:[
        {
          urlImage: uno,
          title: "DIGITAL COMICS"
        },
        {
          urlImage: due,
          title: "DC MERCHANDISE"
        },
        {
          urlImage: tre,
          title: "SUBSCRIPTION"
        },
        {
          urlImage: quatro,
          title: "COMIC SHOP LOCATOR"
        },
        {
          urlImage: cinque,
          title: "DC POWER VISA"
        }
      ]
    }
  }

}
</script>

<style lang="scss" scoped>

@import "../assets/style/_vars.scss";
@import "../assets/style/_mixin.scss";

.container-fluid{
  @include center();
  height: 150px;
  background-color: $primary-color;

  .container{
    @include center();

    .digital-dc{
      @include between();
      margin-right: 45px;
      img{
        width: 30px;
        margin: 15px;
      }

      p{
        font-size: 12px;
        color: white;
        margin-bottom: 0;
      }
    }
  }
  
}

</style>