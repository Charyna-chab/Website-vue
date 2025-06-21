<template>
   
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 p-6 ml-9">
    <PlantCard
      v-for="plant in plants"
      :key="plant.title"
      :title="plant.title"
      :description="plant.description"
      :price="plant.price"
      :image="plant.image"
    />
  </div>
  <Cart/>
</template>

<script setup>
import PlantCard from '@/components/PlantCard.vue';
import Cart from '@/components/Cart.vue';

const plants = [
  {
    title: 'Green Money Plant',
    description: 'plant that purifies air and thrives in low light.',
    price: 15.99,
    image: 'https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSYlCenUZLlhRjnV551Bi8JuJvSXjV_ITnmZh6TdWn6887DisIYpaqIXgFmONuZzY2HpfeHGjE1KVlvYPS0L3LHnw',
  },
  {
    title: 'Plant From Cutting',
    description: 'Popular indoor tree with large, glossy leaves.',
    price: 29.99,
    image: 'https://i.pinimg.com/736x/b0/3b/71/b03b71fb0758410fc853852a359df8d9.jpg',
  },
  {
    title: 'Plant From Cutting',
    description: 'Popular indoor tree with large, glossy leaves.',
    price: 29.99,
    image: 'https://i.pinimg.com/736x/01/da/b5/01dab5313132c43ad074d713bcca9ca7.jpg',
  },
  {
    title: 'Plantas From Cutting',
    description: 'Popular indoor tree with large, glossy leaves.',
    price: 29.99,
    image: 'https://i.pinimg.com/736x/f2/07/07/f207077785b23483fea936160f5d20f5.jpg',
  },
    {
        title: 'Elegant Peace Lily',
        description: 'Popular indoor tree with large, glossy leaves.',
        price: 29.99,
        image: 'https://i.pinimg.com/736x/2c/1f/c0/2c1fc011e77f054f56a2992815f8e332.jpg',
    },
    {
        title: 'Jade Plant For Indoor',
        description: 'Popular indoor tree with large, glossy leaves.',
        price: 29.99,
        image: 'https://i.pinimg.com/736x/48/5e/1b/485e1b7a24e238c955eea595daab56ea.jpg',
    },
  // You can add more plants here...
];
</script>
