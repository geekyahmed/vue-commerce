<template>
  <div id="app">
    <Navbar />
    <Sidebar />
    <router-view />
  </div>
</template>

<script>
  import Sidebar from './components/shared/Sidebar.vue'
  import Navbar from './components/shared/Navbar.vue'
  export default {
    name: 'App',
    components: {
      Navbar,
      Sidebar
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