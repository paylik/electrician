<template>
  <v-app>
    <v-navigation-drawer app>
      <!-- -->
    </v-navigation-drawer>

    <Header />

    <!-- Sizes your content based upon application components -->
    <v-sheet id="scrolling-techniques-3" class="overflow-y-auto">
      <v-main>
        <v-container fluid>
          <router-view />
        </v-container>
      </v-main>
      <v-container style="height: 40%" class="mt-n16"></v-container>
    </v-sheet>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import Header from "@/components/Header.vue";

export default Vue.extend({
  name: "App",

  components: { Header },

  data: () => ({}),
});
</script>
<style>
html {
  overflow-y: hidden !important;
}
</style>
