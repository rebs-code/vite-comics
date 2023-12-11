<script>
import HeaderComponent from './components/Header/HeaderComponent.vue';
import AppComicContainer from './components/AppComicContainer.vue';
import BlueStripeComponent from './components/BlueStripeComponent.vue';
import FooterComponent from './components/Footer/FooterComponent.vue';
import AppJumboComponent from './components/AppJumboComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    AppComicContainer,
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
    <AppComicContainer></AppComicContainer>
    <BlueStripeComponent></BlueStripeComponent>
    <FooterComponent></FooterComponent>
  </div>
</template>
