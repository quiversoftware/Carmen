<template>
  <section id="articles">
    <v-row>
      <v-col>
        <Article />
      </v-col>
      <v-col>
        <Article />
      </v-col>
      <v-col>
        <Article />
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <Article />
      </v-col>
      <v-col>
        <Article />
      </v-col>
      <v-col>
        <Article />
      </v-col>
    </v-row>
  </section>
</template>

<script>
import Article from '@/components/Article.vue';

export default {
  components: { Article },
  name: 'Articles',
}
</script>
