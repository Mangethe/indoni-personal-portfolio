<template>
  <div class="services">
    <div>Services I provide</div>
    <projects-component />
    <projects-component />
    <projects-component />
    <projects-component />
    <projects-component />
    <projects-component />

  </div>
</template>

<script>
// @ is an alias to /src
import ProjectsComponent from "@/components/ProjectsComponent.vue";
// import ServiceComponent from '../components/ServiceComponent.vue';
export default {
  name: "ProjectsView",
  components: {
    ProjectsComponent
  }
};
</script>
