<template>
  <div class="hello">
    <div class="examplex">
      <vs-navbar color="#1cc164" square text-white center-collapsed v-model="active">
        <template #left>
          <img src="./assets/logo.png" alt="">
        </template>
        <template #right>
          <vs-navbar-item :active="active = 'components'" id="components">Home</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">Products</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">About</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components">Contact</vs-navbar-item>
          <vs-button color="#fff" flat>Login</vs-button>
          <vs-button color="#fff" border>Register</vs-button>
        </template>
      </vs-navbar>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Navbar'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .vs-navbar-item {
    font-size: 1000px;
  }

  img {
    width: 50px;
    height: 50px;
  }
</style>