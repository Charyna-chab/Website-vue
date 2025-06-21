<script setup>
import Header from '@/components/Header.vue';
import Card from '@/components/Card.vue';
</script>

<template>
  <main>
     <header
    class="bg-cover bg-center h-64 flex items-center justify-center text-white"
    style="background-image: url('https://images.unsplash.com/photo-1521334884684-d80222895322?auto=format&fit=crop&w=1470&q=80')"
  >
    <h1 class="text-4xl font-bold bg-black bg-opacity-50 px-6 py-3 rounded-lg shadow-md">
     Embrace the Beauty of Nature
    </h1>
  </header>
  </main>
  <Card/>
</template>
