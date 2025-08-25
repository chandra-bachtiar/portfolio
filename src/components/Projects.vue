<script setup>
import portfolio from '../data/portfolio.json';
const { projects } = portfolio;
</script>

<template>
  <section class="max-w-xl mx-auto p-6">
    <h2 class="text-2xl font-semibold mb-4">Projects</h2>
    <ul class="space-y-4">
      <li v-for="project in projects" :key="project.name" class="border rounded-md p-4 hover:bg-gray-50">
        <a :href="project.url" class="text-blue-600 hover:underline font-medium" target="_blank" rel="noopener noreferrer">{{ project.name }}</a>
        <p class="text-sm text-gray-600 mt-1">{{ project.description }}</p>
      </li>
    </ul>
  </section>
</template>

