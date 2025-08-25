<script setup>
import portfolio from '../data/portfolio.json';
const props = defineProps({
  projects: {
    type: Array,
    default: null,
  },
});
const allProjects = props.projects || portfolio.projects;
</script>

<template>
  <section class="max-w-5xl mx-auto p-6">
    <h2 class="text-2xl font-semibold mb-4">Projects</h2>
    <ul class="grid md:grid-cols-2 gap-4">
      <li
        v-for="project in allProjects"
        :key="project.name"
        class="border rounded-md p-4 hover:shadow-lg transition transform hover:-translate-y-1"
      >
        <a
          :href="project.url"
          class="text-blue-600 hover:underline font-medium"
          target="_blank"
          rel="noopener noreferrer"
          >{{ project.name }}</a
        >
        <p class="text-sm text-gray-600 mt-1">{{ project.description }}</p>
      </li>
    </ul>
  </section>
</template>

