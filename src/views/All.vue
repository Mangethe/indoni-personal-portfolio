<template>
  <div>
    <home />
    <about />
  </div>
</template>

<script>
import Home from "@/views/Home.vue";
import About from "@/views/About.vue";
export default {
  name: "All",
  components: {
    Home,
    About
  }
  
}
</script>
