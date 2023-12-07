<script>
// @ts-ignore
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import BlueStripeComponent from './components/BlueStripeComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueStripeComponent
  }
}
</script>

<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <MainComponent></MainComponent>
    <BlueStripeComponent></BlueStripeComponent>
  </div>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>
