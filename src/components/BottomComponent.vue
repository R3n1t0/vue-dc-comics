<template>

  <div class="bottom container-fluid">
    <div class="container">
      <button>SIGN-UP NOW!!</button>

      <div class="social">
        <h5>FOLLOW US</h5>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
      </div>
    </div>  
  </div>
  
</template>

<script>
export default {
  name: "BottomComponent"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/_vars.scss";
@import "../assets/style/_mixin.scss";

.bottom{
  height: 110px;
  background-color: #303030;

  .container{
    @include between();
    width: 70%;
    height: 100%;

    button{
      background-color: #303030;
      color: white;
      border: 2px solid $primary-color;
      padding: 8px 13px;
    }

    .social{
      @include between();
      h5{
        color: $primary-color;
        margin-right: 20px;
      }

      img{
        margin-left: 20px;
      }
    }
  }
}

</style>