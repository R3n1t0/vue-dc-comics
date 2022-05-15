<template>
  <footer class="container-fluid">
    <div class="container">
      <div class="credits">
        <div class="dc-shop">
          <h5>DC COMICS</h5> 
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h5>SHOP</h5>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>

        <div class="dc">
          <h5>DC</h5>
          <ul>
            <li>Term of use</li>
            <li>Policy</li>
            <li>Add choice</li>
            <li>Advertising</li>
            <li>Job</li>
            <li>Subscriptions</li>
            <li>Talent workshop</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop help</li>
            <li>Contact us</li>
          </ul>
        </div>

        <div class="dc">
          <h5>SITES</h5>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Univers</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
      </div>

      <div class="immagine">
        
      </div>
    </div>

  </footer>
</template>

<script>
export default {
  name: "FooterComponent"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/_vars.scss";
@import "../assets/style/_mixin.scss";

footer{
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 330px;
  color: white;

  .container{
    @include between();
    width: 75%;
    height: 100%;

    .credits{
      width: 40%;
      @include start();

      li{
        font-size: 12px;
        color: gray;
      }
    }

    .immagine{
      background-image: url(../assets/img/dc-logo-bg.png);
      background-size: cover;
      background-position: center;
      width: 45%;
      height: 100%; 
    }
  }
}


</style>