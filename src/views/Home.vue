<template>
    <div>
      <HeaderComponent />
      <MainContentComponent />
      <FooterComponent />
    </div>
  </template>
  
  <script>
  import HeaderComponent from '@/components/HeaderComponent.vue';
  import MainContentComponent from '@/components/MainContentComponent.vue';
  import FooterComponent from '@/components/FooterComponent.vue';
  
  export default {
    name: 'Home',
    components: {
      HeaderComponent,
      MainContentComponent,
      FooterComponent,
    },
  };
  </script>
  