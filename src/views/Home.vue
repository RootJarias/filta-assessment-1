<template>
  <CMP_Banner />

  <div class="container mx-auto px-10 pb-[20px] md:px-0">
    <div class="w-full flex justify-between md:block">
      <CMP_Card
        class="m-4"
        v-for="(el, i) in cardData"
        :key="i"
        :image="el.image"
        :author="el.author"
        :description="el.description"
      />
    </div>
  </div>
</template>

<script setup>
// Base Imports
import { ref } from 'vue';

// Import Components
import CMP_Banner from '../components/misc/Banner.vue';
import CMP_Card from '../components/misc/Card.vue';

// Set Datas
const cardData = ref([
  {
    image: '400x300.png',
    author: 'Powered by HTML.COM',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
  },
  {
    image: '400x300.png',
    author: 'Powered by HTML.COM',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
  },
  {
    image: '400x300.png',
    author: 'Powered by HTML.COM',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.',
  },
]);
</script>
