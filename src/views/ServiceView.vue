<template>
    <header
    class="bg-cover bg-center h-64 flex items-center justify-center text-white"
    style="background-image: url('https://i.pinimg.com/736x/54/b9/93/54b9938ba425deb684718c7453cae826.jpg')"
  >
    <h1 class="text-4xl font-bold bg-black bg-opacity-50 px-6 py-3 rounded-lg shadow-md">
    🌿 Our Plant Services
    </h1>
  </header>
  <section class="bg-green-50 py-12">
    <div class="max-w-6xl mx-auto px-4">
      <h2 class="text-3xl font-bold text-green-700 text-center mb-10">🌿 Our Plant Services</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div
          v-for="service in services"
          :key="service.id"
          class="bg-white shadow-md rounded-xl p-6 hover:shadow-lg transition"
        >
          <img :src="service.icon" alt="" class="h-16 w-16 mb-4">
          <h3 class="text-xl font-semibold text-green-800 mb-2">{{ service.title }}</h3>
          <p class="text-gray-600">{{ service.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const services = [
  {
    id: 1,
    title: 'Indoor Plant Installation',
    description: 'We help you select and place the perfect indoor plants for your space.',
    icon: 'https://cdn-icons-png.flaticon.com/512/2909/2909768.png',
  },
  {
    id: 2,
    title: 'Plant Maintenance',
    description: 'Regular care including watering, pruning, and pest control.',
    icon: 'https://cdn-icons-png.flaticon.com/512/2909/2909803.png',
  },
  {
    id: 3,
    title: 'Custom Planters & Styling',
    description: 'Stylish pots and creative designs to match your décor.',
    icon: 'https://cdn-icons-png.flaticon.com/512/2909/2909795.png',
  },
  {
    id: 4,
    title: 'Office Plant Design',
    description: 'Greener workspaces that reduce stress and boost productivity.',
    icon: 'https://cdn-icons-png.flaticon.com/512/2909/2909805.png',
  },
  {
    id: 5,
    title: 'Plant Gifting',
    description: 'Send a green gift for birthdays, celebrations, or corporate events.',
    icon: 'https://cdn-icons-png.flaticon.com/512/2909/2909816.png',
  },
  {
    id: 6,
    title: 'Outdoor Garden Setup',
    description: 'From balcony pots to backyard gardens—we help it bloom.',
    icon: 'https://cdn-icons-png.flaticon.com/512/7662/7662143.png',
  },
];
</script>