<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent
  }
}
</script>

<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <MainComponent></MainComponent>
  </div>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>
