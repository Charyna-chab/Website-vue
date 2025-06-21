<template>
  <div class="">
    <nav class="bg-gray-800 text-white p-4 flex items-center">
      <RouterLink to="/" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" :class="{ 'bg-gray-900 text-white': $route.path === '/' }">Home</RouterLink>
      <RouterLink to="/about" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" :class="{ 'bg-gray-900 text-white': $route.path === '/about' }">About</RouterLink>
      <RouterLink to="/service" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" :class="{ 'bg-gray-900 text-white': $route.path === '/service' }">Service</RouterLink>
      <RouterLink to="/contact" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white" :class="{ 'bg-gray-900 text-white': $route.path === '/contact' }">Contact</RouterLink>
    </nav>
  </div>
</template>

<script>
export default {
  // No additional script needed for this basic implementation
};
</script>