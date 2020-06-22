<template>
  <v-app light>
    <AppBar />
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer absolute app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
import AppBar from '@/components/core/AppBar.vue'

export default {
  components: { AppBar },
  comments: {
    AppBar,
  },

  data() {
    return {}
  },
}
</script>
