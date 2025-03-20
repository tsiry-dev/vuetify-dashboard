<template>
  <v-app-bar flat density="compact">
    <v-spacer></v-spacer>
      <v-tabs>
        <v-tab v-for="(link, index) in links" :key="index">
          {{ link }}
        </v-tab>
      </v-tabs>
    <v-spacer></v-spacer>
  </v-app-bar>

  <v-main>
      <v-container fluid>
        HELLO
      </v-container>
  </v-main>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

const selectedTab = ref(0);
const links = ref(['Dashboard', 'About']);

</script>
