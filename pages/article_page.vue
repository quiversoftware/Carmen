<template>
  <v-layout>
    <v-flex class="text-center">
      <v-container>
        <v-row class="pt-8">
          <v-col cols="12" md="2" class="d-none d-md-block">
            <div class="left_fixed">
              <LeftBar />
            </div>
          </v-col>
          <v-col cols="12" md="8" sm="12" class="px-6 mx-6">
            <v-row>
              <v-col align="left" class="pb-0">
                <h1>THE TITLE OF ARTICLE</h1>
                <h3>The article abstract</h3>
              </v-col>
            </v-row>
            <v-row class="pt-2 pb-8">
              <SocialMedia />
            </v-row>
            <img
              :src="require('@/assets/articles/matematicas.jpg')"
              alt="Vuetify.js"
              class="mb-5"
            />
            <v-col align="justify">
              <div class="article_body">
                La historia de la educación se ciñe a la división de las edades
                del hombre. En los inicios de la Edad Antigua hay que situar las
                concepciones y prácticas educativas de las culturas india,
                china, egipcia y hebrea. Durante el primer milenio a.C. se
                desarrollan las diferentes paideias griegas. El mundo romano
                asimila el helenismo también en el terreno docente, en especial
                gracias a Cicerón quien fue el principal impulsor de la llamada
                humanitas El fin del Imperio romano de Occidente (476) marca el
                final del mundo antiguo y el inicio de la Edad Media. Se fija el
                final de esta edad en la caída de Constantinopla en 1453. El
                cristianismo, nacido y extendido por el Imperio romano, asume la
                labor de mantener el legado clásico, tamizado, filtrado por la
                doctrina cristiana. De la recuperación plena del saber de Grecia
                y Roma que se produce durante el Renacimiento nace el nuevo
                concepto educativo del Humanismo a lo largo del siglo XVI,
                continuado durante el Barroco por el disciplinarismo pedagógico
                y con el colofón ilustrado del siglo XVIII. En la educación
                Contemporánea nacerán los actuales sistemas educativos,
                organizados y controlados por el Estado.
              </div>
            </v-col>
          </v-col>
          <v-col class="d-none d-md-block" cols="12" md="1">
          </v-col>
        </v-row>
      </v-container>
    </v-flex>
  </v-layout>
</template>

<script>
import SocialMedia from '@/components/article/SocialMedia.vue'
import LeftBar from '@/components/article/LeftBar.vue'

export default {
  components: { SocialMedia, LeftBar },
  name: 'article_page',
}
</script>

<style scoped>
h3 {
  color: #7f828b;
}

.article_body {
  font-size: 1.2em;
}
.left_fixed {
  position: fixed;
  top: 30%;
}
</style>
