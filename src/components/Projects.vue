```vue
<template>
    <section class="projects lg:mb-64 px-4 lg:px-0">
        <div class="fade-in bg-[#2f6661] rounded-3xl shadow-lg px-6 py-10 lg:px-12 lg:py-14">
            <div class="border-2 border-[#ffaf87] rounded-xl px-6 py-2 w-fit mx-auto mt-5 mb-12">
                <h2 class="text-3xl lg:text-4xl font-semibold text-center">
                    Projects
                </h2>
            </div>
            <!-- <div class="h-1 w-20 bg-[#ffaf87] rounded-full mx-auto mt-5 mb-12"></div> -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-16 justify-items-center">
                <ProjectCard v-for="project in projects" :key="project.name" :name="project.name"
                    :summary="project.summary" :link="project.link" />
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';
import ProjectCard from './ProjectCard.vue';
import projectsData from '../data/projects.json';
import useFadeIn from '../composables/fadein';

useFadeIn();

const projects = ref(projectsData);
</script>
