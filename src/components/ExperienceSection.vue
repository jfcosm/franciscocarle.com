<template>
    <section class="experience">
      <h2>Experience</h2>
      <div class="job" v-for="job in jobs" :key="job.id">
        <h3>{{ job.title }}</h3>
        <p>{{ job.description }}</p>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "ExperienceSection",
    data() {
      return {
        jobs: [
          { id: 1, title: "Senior Scrum Master", description: "Leading agile teams at Onikom." },
          { id: 2, title: "Web Developer", description: "Building solutions with Python and Django." },
          // Añade más experiencias aquí
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .experience {
    padding: 40px;
    background-color: #fff;
  }
  .experience h2 {
    color: #4CAF50;
  }
  .job {
    margin: 20px 0;
  }
  </style>
  