<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

</script>
<template>
  <header>
    <Navbar/>
  </header>
   <main class="min-h-screen">
    <RouterView /> <!-- this is where views will switch -->
  </main>
  <footer> <Footer/></footer>
</template>

