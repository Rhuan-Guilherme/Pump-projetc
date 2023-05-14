<script setup lang="ts">
  import NavbarComponentVue from './components/NavbarComponent.vue';
  import { onMounted } from 'vue'
  import { initFlowbite } from 'flowbite'

  onMounted(() => {
      initFlowbite();
  })
</script>

<template>
  <NavbarComponentVue/>
  <RouterView />
</template>


