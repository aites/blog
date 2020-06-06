<template>
  <v-container>
    <v-card class="mx-auto" max-width="344">
      <Tweet id="1268497591857111040" :options="{ theme: 'light' }" />
      <v-card-actions>
        <v-spacer></v-spacer>
        メモを記載
        <v-btn icon @click="show = !show">
          <v-icon>{{ show ? "mdi-chevron-up" : "mdi-chevron-down" }}</v-icon>
        </v-btn>
      </v-card-actions>
      <v-expand-transition>
        <div v-show="show">
          <v-divider></v-divider>
          <v-card-text>メモを記載</v-card-text>
        </div>
      </v-expand-transition>
    </v-card>
  </v-container>
</template>

<script>
import { Tweet } from "vue-tweet-embed";

export default {
  name: "blog",
  components: {
    Tweet,
  },
  data: () => ({
    show: false,
    user_id: "2F1268497591857111040",
  }),
};
</script>
