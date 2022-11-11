<template>
  <div class="bg-section">
    <div class="container">
      <div class="list">
        <ListFooter v-for="(item, index) in ArrayFooter" :key="index" :obj="item" />
      </div>
      <img src="../../img/dc-logo-bg.png" alt="logo-bg">
    </div>
  </div>
  <div class="section-social">
    <div class="container">
      <div>
        <button><a href="#nogo">sign-up now!</a></button>
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
import { ArrayFooter } from '../data/dc-comics'
import ListFooter from './ListFooter.vue';
export default {
  name: "FooterComponent",
  data() {
    return {
      ArrayFooter: ArrayFooter
    };
  },
  components: { ListFooter }
}
</script>

<style lang="scss">
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
      flex-wrap: wrap;

      .listMenu {
        width: calc(100%/3);
      }

      .listMenu:last-child {
        margin-top: -50px;
      }
    }

    h3 {
      color: white;
      text-transform: uppercase;
      margin-bottom: 13px;
    }

    ul {
      list-style: none;
      margin-right: 30px;

      li a {
        text-decoration: none;
        color: rgb(152, 150, 149);
        font-size: 0.8rem;
        margin-bottom: 4px;

        &:hover {
          color: white;
        }
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
      border: 3px solid $bluetext;
      background-color: rgb(48, 48, 48);
      padding: 15px;
      font-size: 1rem;

      &:hover {
        background-color: $bluetext;
      }

      a {
        text-decoration: none;
        font-weight: bold;
        text-transform: uppercase;
        color: white;
      }
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

      a img:hover {
        background-color: white;
        border-radius: 100%;
      }
    }
  }
}
</style>