<template>
  <div class="container">
    <h1>Content goes here!</h1>
  </div>
</template>

<script>
export default {

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
</style>