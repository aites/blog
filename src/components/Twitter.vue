<template>
  <v-container>
    <v-card class="mx-auto" max-width="344" outlined>
      <Timeline id="kakun_triplei" source-type="profile" widget-class="mt-3 my-custom-class"></Timeline>
    </v-card>
  </v-container>
</template>

<script>
import { Timeline } from "vue-tweet-embed";

export default {
  name: "twitter",
  components: {
    Timeline
  },
  data: () => ({
    show: false,
    user_id: "2F1268497591857111040"
  })
};
</script>
