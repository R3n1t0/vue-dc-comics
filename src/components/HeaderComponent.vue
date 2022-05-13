<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="DC Logo">
    <nav>
      <ul>
        <li>
          <a href="#">CHARACTERS</a>
        </li>
        <li>
          <a href="#">COMICS</a>
        </li>
        <li>
          <a href="#">MOVIES</a>
        </li>
        <li>
          <a href="#">TV</a>
        </li>
        <li>
          <a href="#">GAMES</a>
        </li>
        <li>
          <a href="#">COLLECTIBLES</a>
        </li>
        <li>
          <a href="#">VIDEOS</a>
        </li>
        <li>
          <a href="#">FANS</a>
        </li>
        <li>
          <a href="#">NEWS</a>
        </li>
        <li>
          <a href="#">SHOP</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>

export default {
  name: "HeaderComponent"
}
</script>

<style lang="scss" scoped>
  @import "../assets/style/_vars.scss";
  @import "../assets/style/_mixin.scss";

  header{
    @include between();
    height: 140px;
    img{
      width: 80px;
      height: 80px;
    }
    ul{
      @include between();
      list-style: none;
      li{
        padding: 25px 15px; 
        &:hover{
          outline: 5px solid $primary-color;
        }
        a{
        text-decoration: none;
        color: black;
        font-size: 10px;
        font-weight: bold;
        }
      }
      
    }
    
  }

</style>