<template>
  <div id="app">
    <NavigationMenu></NavigationMenu>
    <CarouselBanner></CarouselBanner>
    <Gallery></Gallery>
    <TwoPaneGallery></TwoPaneGallery>
  </div>
</template>

<script>
import CarouselBanner from './components/CarouselBanner.vue'
import Gallery from './components/Gallery.vue'
import TwoPaneGallery from './components/TwoPaneGallery.vue'
import NavigationMenu from './components/NavigationMenu.vue'
import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

// Import Bootstrap an BootstrapVue CSS files (order is important)
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

// Make BootstrapVue available throughout your project
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)

export default {
  name: 'App',
  components: {
    NavigationMenu,
    CarouselBanner,
    Gallery,
    TwoPaneGallery
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
