<template>
  <v-app>
    <v-main>
      <v-app-bar app color="#23232F">
        <v-toolbar-title>Most Used Words</v-toolbar-title>
      </v-app-bar>
      <Home />
    </v-main>
  </v-app>
</template>

<script>
import Home from "./components/Home.vue";
export default {
  name: "App",

  components: {
    Home,
  },
};
</script>

<style></style>
