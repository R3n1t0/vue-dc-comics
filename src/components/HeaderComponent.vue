<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="DC Logo">
    <nav>
      <ul>
        <li v-for="(item, index) in opzioniMenu" :key="`menu-${index}`">
          <a :href="item.href">{{item.name}}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>

export default {
  name: "HeaderComponent",

   data(){
    return{
      opzioniMenu: [
        {
          name: "CHARACTERS",
          href: "#",
          isActive: false
        },
        {
          name: "COMICS",
          href: "#",
          isActive: true
        },
        {
          name: "MOVIES",
          href: "#",
          isActive: false
        },
        {
          name: "TV",
          href: "#",
          isActive: false
        },
        {
          name: "GAMES",
          href: "#",
          isActive: false
        },
        {
          name: "COLLECTIBLES",
          href: "#",
          isActive: false
        },
        {
          name: "VIDEOS",
          href: "#",
          isActive: false
        },
        {
          name: "FANS",
          href: "#",
          isActive: false
        },
        {
          name: "NEWS",
          href: "#",
          isActive: false
        },
        {
          name: "SHOP",
          href: "#",
          isActive: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../assets/style/_vars.scss";
  @import "../assets/style/_mixin.scss";

  header{
    @include between();
    width: 80%;
    height: 140px;
    img{
      width: 80px;
      height: 80px;
    }
    ul{
      @include between();
      list-style: none;
      a{
        text-decoration: none;
        color: black;
        font-size: 10px;
        font-weight: bold;
        padding: 0px 15px;
        &:hover{
          color: $primary-color;
        }
      }
 
    }
    
  }

</style>