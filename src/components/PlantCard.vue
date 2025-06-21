<template>
  <div class="max-w-sm bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-300">
    <img
      :src="image"
      :alt="title"
      class="w-full h-56 object-cover"
    />
    <div class="p-5">
      <h2 class="text-2xl font-semibold text-green-700 mb-1">{{ title }}</h2>
      <p class="text-gray-600 text-sm mb-4">{{ description }}</p>
      <div class="flex items-center justify-between">
        <span class="text-lg font-bold text-green-600">${{ price }}</span>
        <button
          @click="order"
          class="bg-green-600 text-white px-4 py-2 rounded-md hover:bg-green-700 transition"
        >
          Order Now
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  price: Number,
  image: String,
})

const order = () => {
  alert('🌱 Your plant has been added to the cart!');
};
</script>
