<template>
  <v-app light>
    <AppBar/>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
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
