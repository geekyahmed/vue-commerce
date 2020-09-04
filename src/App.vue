<template>
  <div id="app">
    <Navbar />
    <router-view />
  </div>
</template>

<script>
  import Navbar from './components/shared/Navbar.vue'
  export default {
    name: 'App',
    components: {
      Navbar
    }
  }
</script>

<style>
  #app,
  * {
    font-family: 'Poppins Regular', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
</style>