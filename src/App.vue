<template>
  <div class="d-flex">
    <SidebarComponent />
    <NavbarComponent />
  </div>
</template>

<script>
import SidebarComponent from './components/SidebarComponent.vue';
import NavbarComponent from './components/NavbarComponent.vue';
  export default {
    name: 'App',
    components: {
      SidebarComponent,
      NavbarComponent
    }
  }
</script>

<style lang="scss" scoped>

</style>