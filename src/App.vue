<script>
import HeaderComponent from './components/Header/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import BlueStripeComponent from './components/BlueStripeComponent.vue';
import FooterComponent from './components/Footer/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueStripeComponent,
    FooterComponent
  }
}
</script>

<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <MainComponent></MainComponent>
    <BlueStripeComponent></BlueStripeComponent>
    <FooterComponent></FooterComponent>
  </div>
</template>
