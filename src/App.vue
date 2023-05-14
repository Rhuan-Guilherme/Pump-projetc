<script setup lang="ts">
  import NavbarComponentVue from './components/NavbarComponent.vue';
  import TheForm from './components/TheForm.vue'
  import TheCardVue from './components/TheCard.vue';
  import { onMounted } from 'vue'
  import { initFlowbite } from 'flowbite'


  onMounted(() => {
      initFlowbite();
  })
</script>

<template>
  <NavbarComponentVue/>
  <div class="flex items-center justify-center mt-32 pb-20 border-b mb-8">
    <the-form class="w-2/4" />
  </div>
  <div class="flex items-center justify-center ">
    <TheCardVue class="w-5/6"/>
  </div>
  <RouterView />
</template>


