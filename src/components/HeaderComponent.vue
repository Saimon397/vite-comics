<template>
  <div class="container">
    <div class="logo">
      <img src="../../public/img/dc-logo.png" alt="logo-img">
    </div>
    <nav>
      <ul>
        <li v-for="(link, index) in links" :key="index" :class="{ 'active': link.current }">
          <a :href="link.url" :class="{ 'active': link.current }">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#nogo",
          current: false,
        },
        {
          text: "Comics",
          url: "#nogo",
          current: true,
        },
        {
          text: "Movies",
          url: "#nogo",
          current: false,
        },
        {
          text: "Tv",
          url: "#nogo",
          current: false,
        },
        {
          text: "Games",
          url: "#nogo",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#nogo",
          current: false,
        },
        {
          text: "Videos",
          url: "#nogo",
          current: false,
        },
        {
          text: "Fans",
          url: "#nogo",
          current: false,
        },
        {
          text: "News",
          url: "#nogo",
          current: false,
        },
        {
          text: "Shop",
          url: "#nogo",
          current: false,
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
  @include dflex
}


ul {
  @include dflex;

  margin-left: 300px;

  li {
    margin-right: 25px;
    list-style: none;
    text-transform: uppercase;
    font-size: 13px;
    font-weight: bold;

    a {
      text-decoration: none;
      color: $blacktext;
      height: 50px;
      padding-bottom: 50px;

      &.active,
      &:hover {
        color: $bluetext;
        border-bottom: 5px solid $bluetext;
      }
    }
  }
}
</style>