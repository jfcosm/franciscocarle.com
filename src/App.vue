<template>
  <div id="app">
    <header>
      <h1>Francisco Carle</h1>
      <p>Senior Scrum Master & Web Developer</p>
    </header>
    <AboutSection />
    <ExperienceSection />
    <SkillsSection />
  </div>
</template>

<script>
import AboutSection from './components/AboutSection.vue';
import ExperienceSection from './components/ExperienceSection.vue';
import SkillsSection from './components/SkillsSection.vue';

export default {
  name: "App",
  components: {
    AboutSection,
    ExperienceSection,
    SkillsSection,
  },
};
</script>
