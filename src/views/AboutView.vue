<script setup>
import Header from '@/components/Header.vue';
import List from '@/components/List.vue';
import Table from '@/components/Table.vue';
</script>

<template>
  <header
    class="bg-cover bg-center h-64 flex items-center justify-center text-white"
    style="background-image: url('https://i.pinimg.com/736x/e2/6d/35/e26d352c8710bab40b472bca96997506.jpg')"
  >
    <h1 class="text-4xl font-bold bg-black bg-opacity-50 px-6 py-3 rounded-lg shadow-md">
     Natural light feels warm
    </h1>
  </header>
  <div class="bg-gradient-to-br from-green-100 via-white to-green-50 min-h-screen py-10">
    <div class="max-w-5xl mx-auto p-6">
      <h1 class="text-3xl font-bold text-green-700 mb-4 text-center">About Our Plant Services</h1>

      <p class="text-gray-700 mb-6 text-center text-lg">
        Welcome to our plant service center! We are passionate about bringing greenery into your spaces.
        Whether you’re a seasoned plant lover or just starting out, we’re here to help you grow.
      </p>
       <!-- Feature List -->
      <List/>
      <!-- Plant Table -->
      <Table/>
    </div>
     
  </div>
</template>