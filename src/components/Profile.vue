<script setup>
import portfolio from '../data/portfolio.json';
const { profile } = portfolio;
</script>

<template>
  <section class="max-w-xl mx-auto text-center p-6">
    <h1 class="text-3xl font-bold tracking-tight">{{ profile.name }}</h1>
    <p class="text-xl text-gray-600">{{ profile.title }}</p>
    <p class="mt-4 text-gray-700">{{ profile.bio }}</p>
  </section>
</template>

