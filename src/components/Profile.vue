<script setup>
import portfolio from '../data/portfolio.json';
const { profile } = portfolio;
</script>

<template>
  <section class="max-w-2xl mx-auto text-center p-6 space-y-4 animate-fade-in">
    <img :src="profile.photo" :alt="profile.name" class="w-48 h-48 rounded-full mx-auto shadow-lg" />
    <h1 class="text-3xl font-bold tracking-tight">{{ profile.name }}</h1>
    <p class="text-xl text-gray-600">{{ profile.title }}</p>
    <p class="mt-4 text-gray-700">{{ profile.about }}</p>
  </section>
</template>

