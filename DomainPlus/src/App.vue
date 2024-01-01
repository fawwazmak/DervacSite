<script>
import { defineComponent } from 'vue';
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './views/Navbar.vue';
import Footer from './views/Footer.vue';


export default defineComponent({
  components: {Navbar, Footer}
})
</script>

<template>
  <Navbar class="sticky top-0 z-50" />
  <RouterView />
  <Footer />
</template>

<style scoped>

</style>
