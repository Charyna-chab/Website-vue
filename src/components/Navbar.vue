<template>
  <div>
    <nav class="bg-gray-800 text-white p-4 flex items-center justify-between">
      <!-- Navigation Links -->
      <div class="flex space-x-2">
        <RouterLink to="/" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/' }">Home</RouterLink>
        <RouterLink to="/about" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/about' }">About</RouterLink>
        <RouterLink to="/service" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/service' }">Service</RouterLink>
        <RouterLink to="/contact" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" 
          :class="{ 'bg-gray-900 text-white': $route.path === '/contact' }">Contact</RouterLink>
      </div>

      <!-- Logo on the Right -->
      <<div class="flex items-center space-x-2">
  <img
    src="https://i.pinimg.com/736x/1a/fb/15/1afb15e799e4617cfc05a34a5b868a9b.jpg"
    alt="Plant Logo"
    class="w-10 h-10 rounded-full object-cover"
  />
  
</div>

    </nav>
  </div>
</template>

<script>
export default {};
</script>
