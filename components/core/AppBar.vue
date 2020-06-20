<template>
  <v-app-bar
    v-scroll="onScroll"
    :color="!isScrolling ? 'transparent' : 'white'"
    fixed
    :flat="isScrolling ? false : true"
  >
    <v-slide-x-transition>
      <v-img
        v-if="showLogo"
        :src="require('@/assets/logo.png')"
        class="shrink"
        contain
        height="50"
      />
    </v-slide-x-transition>

    <v-spacer />

    <social-media />
  </v-app-bar>
</template>

<script>
import SocialMedia from '@/components/SocialMedia.vue';

export default {
  name: 'AppBar',

  components: {
    SocialMedia,
  },

  data: () => ({
    showLogo: false,
    isScrolling: false,
  }),

  methods: {
    onScroll() {
      const offset = window.pageYOffset
      this.isScrolling = offset > 50
      this.showLogo = offset > 200
    },
  },
}
</script>
