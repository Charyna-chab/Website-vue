<template>
   <h2 class="text-xl font-semibold text-green-600 mb-2">Popular Plants</h2>
    <div class="overflow-x-auto">
      <table class="min-w-full bg-white border border-gray-300 shadow-md rounded-lg">
        <thead class="bg-green-100 text-green-800">
          <tr>
            <th class="py-2 px-4 border-b">Plant Name</th>
            <th class="py-2 px-4 border-b">Category</th>
            <th class="py-2 px-4 border-b">Light Needed</th>
            <th class="py-2 px-4 border-b">Price ($)</th>
          </tr>
        </thead>
        <tbody class="text-gray-700">
          <tr>
            <td class="py-2 px-4 border-b">Monstera Deliciosa</td>
            <td class="py-2 px-4 border-b">Indoor</td>
            <td class="py-2 px-4 border-b">Medium</td>
            <td class="py-2 px-4 border-b">29.99</td>
          </tr>
          <tr>
            <td class="py-2 px-4 border-b">Snake Plant</td>
            <td class="py-2 px-4 border-b">Indoor</td>
            <td class="py-2 px-4 border-b">Low</td>
            <td class="py-2 px-4 border-b">19.99</td>
          </tr>
          <tr>
            <td class="py-2 px-4 border-b">Lavender</td>
            <td class="py-2 px-4 border-b">Outdoor</td>
            <td class="py-2 px-4 border-b">Full Sun</td>
            <td class="py-2 px-4 border-b">14.99</td>
          </tr>
        </tbody>
      </table>
    </div>
</template>