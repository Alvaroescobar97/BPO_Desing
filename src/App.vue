<template>
  <div id="app">
    <Banner />
    <Navbar />

    <router-view></router-view>

    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Banner from './components/Banner.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Banner,
    Footer
  }
}
</script>
