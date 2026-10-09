```vue
<template>
  <div class="project-container">
    <a :href="props.link" class="project-card-link">
      <div class="project-card w-80 rounded-xl shadow-xl">
        <div class="flex justify-center items-center h-full p-12">
          <h1>{{ props.name }}</h1>
        </div>
      </div>
    </a>

    <p class="project-summary">
      {{ props.summary }}
    </p>
  </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps([
  'name',
  'summary',
  'link'
]);
</script>

<style scoped>
.project-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.project-card-link {
  text-decoration: none;
  color: inherit;
}

.project-card {
  height: 20rem;
  background-color: #ff8e72;
  transition: background-color 0.1s;
  cursor: pointer;
}

.project-card:hover {
  background-color: #ed6a5e;
}

.project-summary {
  width: 20rem;
  margin-top: 1rem;
  text-align: left;
  font-weight: 500;
}

h1 {
  font-size: 1.5rem;
  color: #ed6a5e;
}

@media (min-width: 1024px) {
  h1 {
    font-size: 3rem;
  }

  .project-card {
    height: 30rem;
  }

  .project-summary {
    width: 20rem;
  }
}
</style>
