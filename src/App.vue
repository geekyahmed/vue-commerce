<template>
  <div id="app">
    <Navbar />
    <Sidebar />
    <ProductCard />
    <router-view />
  </div>
</template>

<script>
  import Sidebar from './components/shared/Sidebar.vue'
  import Navbar from './components/shared/Navbar.vue'
  import ProductCard from './components/ProductCard.vue'
  export default {
    name: 'App',
    components: {
      Navbar,
      Sidebar,
      ProductCard
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