<template>
  <div class="services">
    <div>Services I provide</div>
    <service-component />
    <service-component />
    <service-component />
    <service-component />
    <service-component />
    <service-component />

  </div>
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
