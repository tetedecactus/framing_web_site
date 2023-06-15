<template>
    <section>
      <Navbar />
      <div class="container mx-auto p-4">
        <slot />
      </div>
      <Footer />
    </section>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  import Navbar from '../components/navbar.vue';
  import Footer from '../components/footer.vue';
  
  //// import Footer from '@/components/Footer.vue'
  export default defineComponent({
    components: {
      Navbar,
      Footer,
    },
  });
  </script>
  
  <style lang="scss" scoped></style>
  