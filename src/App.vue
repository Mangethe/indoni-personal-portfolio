<template>
  <div id="app">
    <navbar-component />
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/services">Services</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/projects">Projects</router-link> |
      <router-link to="/contact">Contact</router-link>
    </div> -->
    <router-view />
  </div>
</template>

<script>
import NavbarComponent from "@/components/NavbarComponent.vue";
export default {
  components: {
    NavbarComponent
  }
  
}
</script>

<style lang="scss">
@import "~@/styles/main.scss";
</style>
