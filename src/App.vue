<script setup>
  import navbar from './components/navbar.vue'
  import about from './components/About.vue'
  import projects from './components/Projects.vue'
  import tools from './components/Tools.vue'
  import contact from './components/Contact.vue'
  import FooterComponent from './components/FooterComponent.vue'
</script>

<template>
  <navbar />
  <div class="container-fluid">
    <about />
    <projects />
    <tools />
    <contact />
  </div>
  <FooterComponent />
</template>
