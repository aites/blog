<template>
  <v-container>
    <v-card class="mx-auto" v-for="blog in blogData" :key="blog">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="headline mb-1">
            {{
            blog.title
            }}
          </v-list-item-title>
          <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-card>
  </v-container>
</template>

<script>
import BlogData from "../data/BlogData";
const blogArray = new BlogData();

export default {
  name: "blog",
  data: () => ({
    blogData: blogArray
  })
};
</script>
