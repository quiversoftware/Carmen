<template>
  <section id="top_articles">
    <v-carousel
      cycle
      height="400"
      hide-delimiter-background
      show-arrows-on-hover
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-sheet height="100%" color="grey">
          <v-row class="fill-height" align="center" justify="center">
            <v-card :height="350" color="grey lighten-1" dark href="#!">
              <v-img
                :src="require('@/assets/articles/matematicas.jpg')"
                height="100%"
                gradient="rgba(0, 0, 0, .42), rgba(0, 0, 0, .42)"
              >
                <v-row class="fill-height text-right ma-0">
                  <v-col cols="12">
                    <v-chip
                      label
                      class="mx-0 mb-2 text-uppercase"
                      color="grey darken-3"
                      text-color="white"
                      small
                      @click.stop=""
                    >
                      Matemáticas
                    </v-chip>

                    <h3 class="title font-weight-bold mb-2">
                      Artículo 1
                    </h3>

                    <div class="caption">
                      Carmen Huertas<br />01/01/2020
                    </div>
                  </v-col>

                  <v-col align-self="end">
                    <v-chip
                      class="text-uppercase ma-0"
                      color="primary"
                      label
                      small
                      @click.stop=""
                    >
                      Read More
                    </v-chip>
                  </v-col>
                </v-row>
              </v-img>
            </v-card>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
  </section>
</template>

<script>
export default {
  name: 'Carousel',
  data() {
    return {
      slides: ['First', 'Second', 'Third', 'Fourth', 'Fifth'],
    }
  },
}
</script>
