<template>
  <v-layout>
    <v-main>
      <section id="hero">
        <v-row no-gutters>
          <v-img
            :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
            :src="require('@/assets/background_image_2.jpg')"
          >
            <v-theme-provider dark>
              <v-container fill-height>
                <v-row
                  align="center"
                  class="white--text mx-auto"
                  justify="center"
                >
                  <v-col class="white--text text-center" cols="12" tag="h1">
                    <span
                      :class="[
                        $vuetify.breakpoint.smAndDown
                          ? 'display-1'
                          : 'display-2',
                      ]"
                      class="font-weight-light"
                    >
                      EL LUGAR DE LA
                    </span>

                    <br />

                    <span
                      :class="[
                        $vuetify.breakpoint.smAndDown
                          ? 'display-3'
                          : 'display-4',
                      ]"
                      class="font-weight-black"
                    >
                      EDUCACIÓN
                    </span>
                  </v-col>

                  <v-btn
                    class="align-self-end"
                    fab
                    outlined
                    @click="$vuetify.goTo('#about-me')"
                  >
                    <v-icon>mdi-chevron-double-down</v-icon>
                  </v-btn>
                </v-row>
              </v-container>
            </v-theme-provider>
          </v-img>
        </v-row>
      </section>
      <AboutMe />
      <EducationalAreas />
      <Phrase />
    </v-main>
  </v-layout>
</template>

<script>
import AboutMe from '@/components/AboutMe'
import EducationalAreas from '@/components/EducationalAreas.vue'
import Phrase from '@/components/Phrase.vue'
export default {
  components: { AboutMe, EducationalAreas, Phrase },
}
</script>

<style scoped>
.header-text {
  color: #35495e;
}
</style>
