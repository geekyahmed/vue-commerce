<template>
  <div id="app">
    <Navbar />
    <ProductCard />
    <router-view />
    <Pagination />
  </div>
</template>

<script>
  import Navbar from './components/shared/Navbar.vue'
  import ProductCard from './components/ProductCard.vue'
  import Pagination from './components/Pagination.vue'

  export default {
    name: 'App',
    components: {
      Navbar,
      ProductCard,
      Pagination
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