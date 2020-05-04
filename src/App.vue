<template>
  <div id="app">
    <Navigation />
    <!-- <Home /> -->
    <!-- <router-link to="/">Home</router-link> | -->
    <!-- <router-link to="/Home">Home</router-link> -->
    <router-view/>
    <Footer />
  </div>
</template>
<script>
import Navigation from './layouts/Navigation'
// import Home from './views/Home'
import Footer from './layouts/Footer'

export default {
  name: 'App',
  components: {
    Navigation,
    // Home,
    Footer
  }
}
</script>
<style lang="scss">
</style>
