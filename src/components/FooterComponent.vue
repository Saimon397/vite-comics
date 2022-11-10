<template>
  <div class="bg-section">
    <div class="container">
      <div class="list">
        <div class="margin">
          <div class="list1">
            <ul>
              <h3>Dc Comics</h3>
              <li><a href="#nogo">Characters</a></li>
              <li><a href="#nogo">Comics</a></li>
              <li><a href="#nogo">Movies</a></li>
              <li><a href="#nogo">TV</a></li>
              <li><a href="#nogo">Games</a></li>
              <li><a href="#nogo">Videos</a></li>
              <li><a href="#nogo">News</a></li>
            </ul>
          </div>
          <div class="list2">
            <ul>
              <h3>Shop</h3>
              <li><a href="#nogo">Shop DC Collectibles</a></li>
              <li><a href="#nogo">Shop DC</a></li>
            </ul>
          </div>
        </div>
        <div class="list3">
          <ul>
            <h3>Dc</h3>
            <li><a href="#nogo">Term Of Use</a></li>
            <li><a href="#nogo">Privacy policy (New)</a></li>
            <li><a href="#nogo">Ad Choices</a></li>
            <li><a href="#nogo">Advertising</a></li>
            <li><a href="#nogo">Jobs</a></li>
            <li><a href="#nogo">Subscription</a></li>
            <li><a href="#nogo">Talent Workshops</a></li>
            <li><a href="#nogo">CPSC Certificates</a></li>
            <li><a href="#nogo">Ratings</a></li>
            <li><a href="#nogo">Shop Help</a></li>
            <li><a href="#nogo">Contact Us</a></li>
          </ul>
        </div>
        <div class="list4">
          <ul>
            <h3>Site</h3>
            <li><a href="#nogo">DC</a></li>
            <li><a href="#nogo">MAD Magazine</a></li>
            <li><a href="#nogo">DC Kids</a></li>
            <li><a href="#nogo">DC Universe</a></li>
            <li><a href="#nogo">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <img src="../../img/dc-logo-bg.png" alt="logo-bg">
    </div>
  </div>
  <div class="section-social">
    <div class="container">
      <div>
        <button>sign-up now!</button>
      </div>
      <div class="social-img">
        <span>follow us</span>
        <a href="#nogo"><img src="../../img/footer-facebook.png" alt="logo-fb"></a>
        <a href="#nogo"><img src="../../img/footer-twitter.png" alt="logo-tw"></a>
        <a href="#nogo"><img src="../../img/footer-youtube.png" alt="logo-yt"></a>
        <a href="#nogo"><img src="../../img/footer-pinterest.png" alt="logo-pint"></a>
        <a href="#nogo"><img src="../../img/footer-periscope.png" alt="logo-per"></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.bg-section {
  background-image: url(../../img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;

  .container {
    @include dflex;
    height: 55vh;
    justify-content: space-between;

    .list {
      display: flex;

      .margin {
        margin-right: 25px;
      }

      .list2 {
        margin-top: 25px;
      }
    }

    h3 {
      color: white;
      text-transform: uppercase;
      margin-bottom: 15px;
    }

    ul {
      list-style: none;
      margin-right: 30px;

      li a {
        display: inline-block;
        text-decoration: none;
        color: rgb(152, 150, 149);
        @include dflex;
        justify-content: flex-start;
        font-size: 0.8rem;
        margin-bottom: 4px;
      }
    }

  }
}

.section-social {
  background-color: rgb(48, 48, 48);

  .container {
    @include dflex;
    height: 100px;
    justify-content: space-between;

    button {
      border: 2px solid $bluetext;
      background-color: rgb(48, 48, 48);
      padding: 15px;
      font-size: 1rem;
      text-transform: uppercase;
      color: white;
    }

    .social-img {
      @include dflex;

      span {
        color: $bluetext;
        font-weight: bold;
        text-transform: uppercase;
        font-size: 1.2rem;
      }

      span,
      img {
        margin-right: 20px;
      }
    }
  }
}
</style>