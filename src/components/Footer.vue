<script setup>
import portfolio from '../data/portfolio.json';
const { socials, profile } = portfolio;
</script>

<template>
  <footer class="bg-gray-100 mt-12">
    <section class="max-w-5xl mx-auto p-6 text-center">
      <h2 class="text-lg font-semibold mb-2">Find me on</h2>
      <ul class="flex justify-center space-x-4">
        <li v-for="(url, network) in socials" :key="network">
          <a :href="url" class="text-blue-600 hover:underline" target="_blank" rel="noopener noreferrer">{{ network }}</a>
        </li>
      </ul>
      <p class="mt-6 text-sm text-gray-500">&copy; {{ new Date().getFullYear() }} {{ profile.name }}</p>
    </section>
  </footer>
</template>
