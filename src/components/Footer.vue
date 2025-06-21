<template>
  <footer class="bg-gradient-to-r from-green-700 to-emerald-600 text-white py-10">
    <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-3 gap-8">
      
      <!-- Logo / About -->
      <div>
        <h2 class="text-2xl font-bold mb-2">🌱 Plantify</h2>
        <p class="text-sm text-gray-200">
          Your one-stop shop for beautiful, air-purifying plants delivered to your doorstep.
        </p>
      </div>

      <!-- Navigation Links -->
      <div>
        <h3 class="text-xl font-semibold mb-3">Quick Links</h3>
        <ul class="space-y-2 text-gray-100">
           <RouterLink to="/" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/' }">Home</RouterLink>
        <RouterLink to="/about" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/about' }">About</RouterLink>
        <RouterLink to="/service" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/service' }">Service</RouterLink>
        <RouterLink to="/contact" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/contact' }">Contact</RouterLink>
     
        </ul>
      </div>

      <!-- Social Icons -->
      <div>
        <h3 class="text-xl font-semibold mb-3">Follow Us</h3>
        <h1>charyna.chab@student.passerellesnumeriques.org</h1>
      </div>

    </div>

    <!-- Bottom note -->
    <div class="text-center text-gray-300 mt-8 text-sm">
     Bring life to your space — one plant at a time.
    </div>
  </footer>
</template>

<!-- Font Awesome (optional) -->
<script>
  // If you're not already including FontAwesome in your app:
  // Install via CDN or npm for icons to work.
</script>
