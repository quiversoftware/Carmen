<template>
  <section id="stats">
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 700 : 500"
      :src="require('@/assets/background_image.jpg')"
    >
      <v-container fill-height>
        <v-row class="mx-auto">
          <v-col>
            <div class="text-center">
              <div class="display-3 font-weight-black mb-4">
                {{ parallax_title }}
              </div>

              <div class="title font-weight-regular text-uppercase">
                {{ parallax_text }}
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-parallax>
  </section>
</template>

<script>
export default {
  name: 'Phrase',
  data() {
    return {
      parallax_title:
        '"En cuestiones de cultura y de saber, sólo se pierde lo que se guarda; sólo se gana lo que se da"',
      parallax_text: '- Antonio Machado',
    }
  },
}
</script>
