<template>
  <div id="app">
    <header>
      <h1>Francisco Carle</h1>
      <p>Senior Scrum Master & Web Developer</p>
    </header>
    <AboutSection />
  </div>
</template>

<script>
import AboutSection from './components/AboutSection.vue';

export default {
  name: "App",
  components: {
    AboutSection,
  },
};
</script>

<style>
/* Global Styles can go here */
</style>
