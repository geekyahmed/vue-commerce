<template>
  <div class="hello">
    <div class="examplex">
      <vs-navbar color="#1cc164" square text-white class="navbarx" v-model="active">
        <template #left>
          <img src="./assets/logo.png" alt="">
        </template>
        <template #right>
          <vs-navbar-item :active="active = 'components'" :style="sizeStyle" id="components">Home</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components" :style="sizeStyle">Products</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components" :style="sizeStyle">About</vs-navbar-item>
          <vs-navbar-item :active="active = 'components'" id="components" :style="sizeStyle">Contact</vs-navbar-item>
          <vs-button color="#fff" flat :style="sizeStyle">Login</vs-button>
          <vs-button color="#fff" border :style="sizeStyle">Register</vs-button>
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
        sizeStyle: {
          fontSize: "13px"
        }
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #vs-navbar-item {
    font-size: 1000px;
  }

  img {
    width: 50px;
    height: 50px;
  }
</style>