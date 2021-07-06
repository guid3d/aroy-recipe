<template>
  <v-container>
    <recipe-list />
  </v-container>
</template>

<script>
import RecipeList from "../components/RecipeList.vue";

export default {
  name: "Home",

  components: {
    RecipeList,
  },
};
</script>
