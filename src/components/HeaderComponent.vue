<template>
  <div>

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
</style>