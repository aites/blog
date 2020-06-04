<template>
  <v-container>
    <v-card class="mx-auto" max-width="344">
      <Tweet id="1268497591857111040" :options="{ theme: 'light' }" />

      <v-expand-transition>
        <div v-show="show">
          <v-divider></v-divider>

          <v-card-text
            >I'm a thing. But, like most politicians, he promised more than he
            could deliver. You won't have time for sleeping, soldier, not with
            all the bed making you'll be doing. Then we'll go with that data
            file! Hey, you add a one and two zeros to that or we walk! You're
            going to do his laundry? I've got to find a way to
            escape.</v-card-text
          >
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
