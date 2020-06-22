<template>
  <section id="education_areas" class="grey lighten-3">
    <v-container class="text-center" py-10>
      <h2 class="display-2 font-weight-bold mb-3">ÁREAS DE LA EDUCACIÓN</h2>
      <v-responsive class="mx-auto mb-12" width="56">
        <v-divider class="mb-1"></v-divider>
        <v-divider></v-divider>
      </v-responsive>
      <v-row py-12>
        <v-col
          v-for="({ icon, title, text }, i) in education_areas"
          :key="i"
          cols="12"
          md="4"
        >
          <v-card class="py-12 px-4" color="grey lighten-5" flat>
            <v-theme-provider dark>
              <v-avatar color="primary" size="80">
                <v-icon large v-text="icon"></v-icon>
              </v-avatar>
            </v-theme-provider>
            <v-card-title
              class="justify-center font-weight-black text-uppercase"
              v-text="title"
            ></v-card-title>
            <v-card-text class="subtitle-1" v-text="text"> </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  name: 'EducationalAreas',
  data() {
    return {
      education_areas: [
        {
          title: 'Matemáticas',
          icon: 'mdi-chess-rook',
          text:
            'El aprendizaje de las matemáticas requiere de una comprensión relacional e instrumental de la ' +
            'Matemática, que estimule la intuición científica y desarrolle un pensamiento lógico en los estudiantes ' +
            'y facilite el uso creativo de principios de aplicación general para la resolución de problemas.',
        },
        {
          title: 'Comunicación-Arte',
          icon: 'mdi-flower-outline',
          text:
            'En esta área, corresponde al enfoque pos-moderno (multicultural e interdisciplinario). Este enfoque ' +
            'propone nuevas respuestas pedagógicas que reconocen las características sociales y ' +
            'culturales de la producción artística como herramienta de identidad ',
        },
        {
          title: 'Ciencias',
          icon: 'mdi-chemical-weapon',
          text:
            'Encontrar el sentido de cómo funciona el mundo natural y el mundo diseñado por el hombre, para pensar ' +
            'de forma crítica e independiente, para reconocer y sopesar explicaciones alternativas sobre los ' +
            'eventos y reconocer y sopesar también las ventajas y desventajas de distintas opciones de diseño.',
        },
      ],
    }
  },
}
</script>
