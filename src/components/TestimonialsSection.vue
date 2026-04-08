<template>
  <section id="testimonios" class="testimonials-section">
    <h2>Lo que dicen de mí</h2>
    <div class="testimonials-container">
      
      <div v-for="(testimonial, index) in testimonials" :key="index" class="testimonial-card">
        <p class="testimonial-text">"{{ testimonial.text }}"</p>
        <div class="testimonial-author">
          <strong>{{ testimonial.name }}</strong>
          <span>{{ testimonial.role }}</span>
        </div>
      </div>
      
    </div>
  </section>
</template>

<script>
export default {
  name: 'TestimonialsSection',
  data() {
    return {
      testimonials: [
        {
          name: "Bruno Rimassa",
          role: "Product Owner - Gasco",
          text: "De mis 7 años trabajando con metodologías ágiles y Scrum, debo decir que Francisco es uno de los mejores Scrum Master con los que he tenido la suerte de trabajar. Muy proactivo, resolutor, excelente en la gestión de equipos, siempre buscando la mejora en pro de conseguir los objetivos."
        },
        {
          name: "Paulina Carvajal Muñoz",
          role: "Ingeniera Civil Industrial",
          text: "La frase 'excelente profesional' queda pequeña para definir a Francisco. Su especialidad como Scrum Master logra que los equipos mantengan un ritmo de trabajo y ambiente excepcional. Es comprometido con su trabajo, tiene una creatividad increíble y es capaz de resolver problemas de forma ágil."
        },
        {
          name: "Stiwart Tobías Antúnez",
          role: "CEO codi-codi.com | Full Stack Developer",
          text: "Su profundo conocimiento de Scrum y su habilidad para liderar equipos en proyectos desafiantes son notables. Francisco lideró con visión estratégica y condujo transformaciones ágiles efectivas. Lo recomiendo sin reservas como Líder de Agilidad y Scrum Master."
        },
        {
          name: "Iván Villarroel Ramirez",
          role: "Backend Engineer | AI Engineer",
          text: "Francisco es un tremendo profesional, inspira a los equipos como pocas personas pueden hacerlo. Su estilo fraterno y cordial le permite facilitar un equipo diverso y enfocarlos en la dirección del objetivo del producto. Su dirección de proyecto y equipo fue impecable."
        }
      ]
    }
  }
};
</script>

<style scoped>
.testimonials-section {
  padding: 50px;
  background-color: #f6f9fc;
  color: #333;
}
.testimonials-section h2 {
  text-align: center;
  margin-bottom: 40px;
}
.testimonials-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  max-width: 1200px;
  margin: 0 auto;
}
.testimonial-card {
  background-color: #ffffff;
  border: 1px solid #e1e4e8;
  border-radius: 8px;
  padding: 25px;
  width: calc(50% - 20px);
  min-width: 300px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.testimonial-text {
  font-style: italic;
  margin-bottom: 20px;
  line-height: 1.6;
  color: #555;
}
.testimonial-author {
  display: flex;
  flex-direction: column;
  border-top: 1px solid #eee;
  padding-top: 15px;
}
.testimonial-author strong {
  font-size: 1.1em;
  color: #2c3e50;
}
.testimonial-author span {
  font-size: 0.9em;
  color: #7f8c8d;
}

@media (max-width: 768px) {
  .testimonial-card {
    width: 100%;
  }
}
</style>
