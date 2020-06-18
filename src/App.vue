<template>
  <v-app>
    <div>
      <v-app-bar color="light-green" dark>
        <v-toolbar-title>かーくん勉強ブログ</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn
          href="https://twitter.com/kakun_triplei?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed&ref_url=http%3A%2F%2Flocalhost%3A8080%2F"
          class="ma-2"
          color="blue"
          ><v-icon color="white">mdi-twitter</v-icon>カーくん</v-btn
        >
      </v-app-bar>
    </div>
    <v-content>
      <Blog />
      <Twitter />
    </v-content>
  </v-app>
</template>

<script>
import Twitter from "./components/Twitter";
import Blog from "./components/Blog";

export default {
  name: "App",

  components: {
    Twitter,
    Blog,
  },

  data: () => ({
    drawer: false,
  }),
};
</script>
