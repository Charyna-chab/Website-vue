<template>
  <div class="flex flex-col md:flex-row bg-gray-50 p-6 mt-5">
    <div class="w-full md:w-2/3">
      <div class="relative">
        <img src="https://i.pinimg.com/736x/9a/06/54/9a0654b6daf21b2a78cabe99685425ee.jpg" alt="Houseplant Journey" class="w-full max-h-72 object-cover">
        <button @click="toggleMute" class="absolute top-6 left-6 bg-black text-white px-4 py-2 rounded hidden">
          Mute
        </button>
      </div>
    </div>
    <div class="w-full md:w-1/3 p-6 flex flex-col justify-center">
      <h2 class="text-lg font-medium text-green-800">LIFE GATHERS AROUND PLANTS</h2>
      <h3 class="text-3xl font-bold text-gray-900">A Houseplant's Journey Home</h3>
      <p class="text-gray-600 mt-4 text-base">Follow along on a Bird of Paradise's journey from our greenhouse to your home, and learn how we care for your plant every step of the way.</p>
      <button @click="learnMore" class="mt-6 bg-green-700 text-white px-8 py-3 rounded-full w-max text-base">LEARN MORE</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    toggleMute() {
      // No action needed since there's no video
    },
    learnMore() {
      alert('Learn more clicked!');
    },
  },
};
</script>