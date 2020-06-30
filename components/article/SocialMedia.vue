<template>
  <v-row align="center">
    <v-row align="center">
      <v-col cols="4" sm="2" md="1">
        <v-avatar size="55px">
          <v-img :src="require('@/assets/carmen_profile.jpg')"></v-img>
        </v-avatar>
      </v-col>
      <v-col class="hidden-xs-only" sm="5" md="5">
        <span class="grey--text">{{ article.author }}</span>
        <span class="grey--text">10/01/2020</span>
      </v-col>
    </v-row>
    <v-spacer></v-spacer>
    <v-col>
      <v-btn icon color="black">
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
      <v-btn icon color="black">
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
      <v-btn icon color="black">
        <v-icon>mdi-heart-outline</v-icon>
      </v-btn>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'SocialMedia',
  data() {
    return {
      article: {
        author: 'Carmen Huertas',
      },
    }
  },
}
</script>
