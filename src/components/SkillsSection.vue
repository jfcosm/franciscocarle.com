<template>
    <section class="skills">
      <h2>Skills</h2>
      <ul>
        <li v-for="skill in skills" :key="skill">{{ skill }}</li>
      </ul>
    </section>
  </template>
  
  <script>
  export default {
    name: "SkillsSection",
    data() {
      return {
        skills: ["Python", "Django", "Agile Methodologies", "Vue.js", "Project Leadership"],
      };
    },
  };
  </script>
  
  <style scoped>
  .skills {
    padding: 40px;
    background-color: #f4f4f9;
  }
  .skills h2 {
    color: #4CAF50;
  }
  .skills ul {
    list-style-type: none;
    padding: 0;
  }
  .skills li {
    margin: 5px 0;
  }
  </style>
  