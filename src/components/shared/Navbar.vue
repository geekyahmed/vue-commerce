<template>
  <div class="hello">
    <div class="examplex">
      <vs-navbar color="#7d33ff" square text-white center-collapsed v-model="active">
        <template #left>
          <h3>Vue-Commerce</h3>
        </template>
        <template #right>
          <vs-navbar-item :active="active = 'components'" id="components">Home</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">Products</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">About</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">Contact</vs-navbar-item>
          <vs-button color="#fff" flat>Login</vs-button>
          <vs-button color="#fff" border>Register Here</vs-button>
        </template>
      </vs-navbar>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Navbar',
    data() {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .vs-navbar-item {
    font-size: 1000px;
  }
</style>