<template>
  <div>
    <HeaderComponent />
    <JumboComponent />
    <MainComponent />
    <Main2Component />
    <FooterComponent />
  </div>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import Main2Component from './components/Main2Component.vue';
import JumboComponent from './components/JumboComponent.vue';
import MainComponent from './components/MainComponent.vue';

export default {
  components: { HeaderComponent, JumboComponent, MainComponent, Main2Component, FooterComponent }
}
</script>

<style lang="scss" scoped>

</style>
