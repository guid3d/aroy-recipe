<template>
  <v-app id="inspire">
    <v-app-bar app color="primary" dark>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Aroy Recipe</v-toolbar-title>
    </v-app-bar>

    <!-- <v-navigation-drawer
      v-model="drawer"
      fixed
      temporary
    >
      
    </v-navigation-drawer> -->

    <v-main class="grey lighten-2">
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({ drawer: null }),
};
</script>
