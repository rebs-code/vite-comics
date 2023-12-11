<script>
import HeaderComponent from './components/Header/HeaderComponent.vue';
import MainComponent from './components/AppMainComponent.vue';
import BlueStripeComponent from './components/BlueStripeComponent.vue';
import FooterComponent from './components/Footer/FooterComponent.vue';
import AppJumboComponent from './components/AppJumboComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueStripeComponent,
    FooterComponent,
    AppJumboComponent
  }
}
</script>

<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <AppJumboComponent></AppJumboComponent>
    <MainComponent></MainComponent>
    <BlueStripeComponent></BlueStripeComponent>
    <FooterComponent></FooterComponent>
  </div>
</template>
