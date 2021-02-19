<template>
  <section class="hero is-fullheight is-justify-content-center bg--white">
    <div class="title mb-3 is-size-2 pt-5">
      <span class="text--secondary-light">Services</span> <span>I provide</span>
      </div>
    <div class="columns is-vcentered is-justify-content-center">
      <div class="column is-8 bg--tertiary-dark p-3">
        <div class="columns">
          <div class="column is-half"><service-component /></div>
          <div class="column is-half"><service-component /></div>
          
        </div>
        <div class="columns">
          <div class="column is-half"><service-component /></div>
          <div class="column is-half"><service-component /></div>
          
        </div>
        <div class="columns">
          <div class="column is-half"><service-component /></div>
          <div class="column is-half"><service-component /></div>
          
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
import ServiceComponent from "@/components/ServiceComponent.vue";
// import ServiceComponent from '../components/ServiceComponent.vue';
export default {
  name: "Service",
  components: {
    ServiceComponent
  }
};
</script>
