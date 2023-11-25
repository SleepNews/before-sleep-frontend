<script setup lang="ts">

</script>

<template>
  <v-container>
    <v-row>
      <v-col cols="2">
        <v-sheet rounded="1g">
          <v-list rounded="1g">
            <v-list-item
              v-for="n in 673"
              :key="n"
              link
              :title="`睡前消息 ${n}`"
            >
            </v-list-item>
          </v-list>
        </v-sheet>
      </v-col>

      <v-col>
        <v-sheet min-height="70vh">

        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>

</style>
