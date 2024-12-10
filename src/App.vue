<template>
  <div id="app">
    <header>
      <nav>
        <ul>
          <li><a href="#inicio">Inicio</a></li>
          <li><a href="#sobre-mi">Sobre Mí</a></li>
          <li><a href="#habilidades">Habilidades</a></li>
          <li><a href="#proyectos">Proyectos</a></li>
          <li><a href="#contacto">Contacto</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <HomeSection />
      <AboutSection />
      <SkillsSection />
      <ProjectsSection />
      <ContactSection />
    </main>
  </div>
</template>

<script>
import HomeSection from './components/HomeSection.vue';
import AboutSection from './components/AboutSection.vue';
import SkillsSection from './components/SkillsSection.vue';
import ProjectsSection from './components/ProjectsSection.vue';
import ContactSection from './components/ContactSection.vue';

export default {
  name: 'App',
  components: {
    HomeSection,
    AboutSection,
    SkillsSection,
    ProjectsSection,
    ContactSection,
  },
};
</script>

<style>
/* Puedes agregar estilos globales aquí o mantener el archivo limpio para solo cargar estilos individuales por componente. */
</style>
