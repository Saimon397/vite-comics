<template>
  <div class="container">
    <h1>Content goes here!</h1>
  </div>
  <div class="container2">
    <ul>
      <li v-for="(img, index) in cont2img" :key="index">
        <a :href="img.url">
          <img :src="img.img" :alt="img.text" class="ico-img">
          <span>{{ img.text }}</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MainComponent',
  data() {
    return {
      cont2img: [
        {
          img: '/img/buy-comics-digital-comics.png',
          text: 'digital comics',
          url: '#nogo'
        },
        {
          img: '/img/buy-comics-merchandise.png',
          text: 'dc merchandise',
          url: '#nogo'
        },
        {
          img: '/img/buy-comics-subscriptions.png',
          text: 'subscription',
          url: '#nogo'
        },
        {
          img: '/img/buy-comics-shop-locator.png',
          text: 'comic shop locator',
          url: '#nogo'
        },
        {
          img: '/img/buy-dc-power-visa.svg',
          text: 'dc power visa',
          url: '#nogo'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.container {
  @include dflex;
  background-color: black;
  justify-content: start;
  max-width: 100%;
  padding: 3rem;

  h1 {
    color: white;
    margin-left: 180px;
  }
}

.container2 {
  @include dflex;
  background-color: $bluetext;
  max-width: 100%;
  padding: 4.5rem;

  ul {
    list-style: none;
    @include dflex;
    padding: 0 30px;

    li a {
      display: inline-block;
      text-decoration: none;
      text-transform: uppercase;
      color: white;
      @include dflex;
      font-size: 0.9rem;

      .ico-img {
        height: 6vh;
      }

      span {
        margin-left: 10px;
        margin-right: 50px;
      }
    }
  }
}
</style>