
<template>
    <!-- My Projects Section -->
    <section class="pb-5" id="projects">
        <!-- Section Heading -->
        <h1 class="mt-5 mb-5 pb-4 text-center">My Projects</h1>

        <!-- Render every project imported from projects.json. -->
        <div class="row justify-content-center">
            <div
                v-for="project in projects"
                :key="project.id"
                class="col-12 col-md-6 col-lg-4 d-flex mb-5"
            >
                <ProjectCard :project="project" />
            </div>
        </div>
    </section>
</template>

<script setup>
// Import the ProjectCard component which will display individual project details
import ProjectCard from './ProjectCard.vue';

// Import the project data from a local JSON file
import projects from '../data/projects.json';
</script>

<style scoped>
:deep(.card) {
    width: 100%;
}
</style>
