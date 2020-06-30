<template>
  <v-container fill-height>
    <v-row align="center" justify="center">
      <v-col>
        <v-row align="center" justify="center">
          <v-avatar size="55px">
            <v-img :src="require('@/assets/carmen_profile.jpg')"></v-img>
          </v-avatar>
        </v-row>
        <v-row align="center" justify="center">
          <span class="grey--text">{{ article.author }}</span>
        </v-row>
        <v-row align="center" justify="center">
          <span class="grey--text">{{ article.description }}</span>
        </v-row>
        <v-row align="center" justify="center">
          <span class="grey--text">10/01/2020</span>
        </v-row>
        <v-row align="center" justify="center">
          <v-chip
            class="ma-2"
            :input-value="following"
            filter
            color="green"
            outlined
            @click="follow"
          >
            {{ follow_text }}
          </v-chip>
        </v-row>
        <v-divider></v-divider>
        <v-row>
          <v-col align="right">
            <v-icon>mdi-thumb-up</v-icon>
          </v-col>
          <v-col align="left">
            {{ article.claps }}
          </v-col>
        </v-row>
        <v-row align="center" justify="center">
          <v-btn icon color="black">
            <v-icon>mdi-heart-outline</v-icon>
          </v-btn>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'LeftBar',
  data() {
    return {
      offsetTop: 0,
      article: {
        author: 'Carmen Huertas',
        description: 'Educadora desde 1980',
        claps: 230,
      },
      following: false,
      follow_text: 'Follow',
    }
  },
  methods: {
    follow() {
      this.following = !this.following
      this.follow_text = this.following ? 'Following' : 'Follow'
    },
  },
}
</script>

<style scoped>
.fixed {
  position: fixed;
}
</style>
