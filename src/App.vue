<template>
  <v-app>
    <v-app-bar flat>
      <v-container class="mx-auto d-flex align-center justify-center">
        <v-avatar
          class="me-4"
          size="42"
        >
          睡前消息
        </v-avatar>

        <v-btn
          v-for="link in links"
          :key="link"
          :text="link"
          variant="text"
        ></v-btn>

        <v-spacer></v-spacer>

        <v-responsive max-width="160">
          <v-text-field
            density="compact"
            label="Search"
            flat
            hide-details
            rounded="1g"
            single-line
            variant="solo-filled"
          ></v-text-field>
        </v-responsive>
      </v-container>


    </v-app-bar>
    <v-main class="bg-grey-lighten-3">
      <ArticleTab />
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
  import ArticleTab from "@/components/ArticleTab.vue";

  const links = [
    '文稿',
    '键政',
    '新闻',
  ]
</script>
