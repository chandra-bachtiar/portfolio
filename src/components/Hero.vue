<script setup>
import portfolio from '../data/portfolio.json';
const { profile } = portfolio;
</script>

<template>
  <section class="text-center py-20 bg-gradient-to-b from-blue-50 to-white animate-fade-in">
    <img :src="profile.photo" :alt="profile.name" class="w-32 h-32 mx-auto rounded-full mb-6 shadow-lg" />
    <h1 class="text-4xl font-bold mb-2">{{ profile.name }}</h1>
    <p class="text-xl text-gray-600">{{ profile.title }}</p>
    <p class="mt-4 max-w-xl mx-auto text-gray-700">{{ profile.bio }}</p>
  </section>
</template>
