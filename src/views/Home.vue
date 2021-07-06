<template>
  <div>
    <v-container>
      <recipe-list />
    </v-container>
    <v-btn
      color="primary"
      elevation="2"
      fab
      class="fab-add-recipe"
      @click="toAddRecipe"
    >
      <v-icon>mdi-plus</v-icon>
    </v-btn>
  </div>
</template>

<script>
import RecipeList from "../components/RecipeList.vue";

export default {
  name: "Home",

  components: {
    RecipeList,
  },

  methods: {
    toAddRecipe() {
      this.$router.push({ name: "AddRecipe" });
    },
  },
};
</script>

<style scoped>
.fab-add-recipe {
  right: 0;
  bottom: 0;
  position: fixed;
  margin: 16px 16px 16px 16px;
}
</style>
