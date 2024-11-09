<!-- layouts/default.vue -->
<template>
    <div>
      <!-- Header -->
      <Header />
  
      <!-- Main content -->
      <NuxtPage />
  
      <!-- Footer -->
      <Footer />
    </div>
  </template>
  
  <script>
  import Header from '~/components/Header.vue'
  import Footer from '~/components/Footer.vue'
  
  export default {
    components: {
      Header,
      Footer
    }
  }
  </script>
  
  <style scoped>
  /* Add styles for layout if necessary */
  </style>
  