<template>
  <section id="about-me">
    <div class="py-12"></div>

    <v-container class="text-center">
      <h2 class="display-2 font-weight-bold mb-3">
        Kids are the digital native
      </h2>

      <v-responsive class="mx-auto mb-8" width="56">
        <v-divider class="mb-1"></v-divider>

        <v-divider></v-divider>
      </v-responsive>

      <v-responsive
        class="mx-auto title font-weight-light mb-8"
        max-width="720"
      >
        Kids know technology better than most adults. It has become the easiest
        easiest way they learn, because it is such an integral part of their
        Engaging with technology in the classroom has not only helped them learn
        but they also acquire multi-tasking skills. At this day in age, they
        they hardly know how to learn without it. This knowledge is important,
        because they would be way behind in the real world without it.
      </v-responsive>

      <v-avatar class="elevation-12 mb-12" size="128">
        <v-img :src="require('@/assets/carmen_profile.jpg')"></v-img>
      </v-avatar>

      <div></div>
    </v-container>

    <div class="py-12"></div>
  </section>
</template>

<script>
export default {
  name: 'AboutMe',
}
</script>
