<template>
  <div class="bg-section">
    <ul>
      <h4></h4>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
    </ul>
    <ul>
      <h4></h4>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
    </ul>
    <ul>
      <h4></h4>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
    </ul>
    <ul>
      <h4></h4>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
      <li><a href="#nogo"></a></li>
    </ul>
    <img src="../../img/dc-logo-bg.png" alt="logo-bg">
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
  max-width: 100%;
  background-image: url(../../public/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
  @include dflex;
  justify-content: space-between;
}
</style>