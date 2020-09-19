<template>
  <v-container grid-list-md fluid>
    <v-layout wrap>
      <v-flex xs12 sm4 md3 v-for="dog in dogs" :key="dog.breed">
        <app-pet :pet="dog"></app-pet>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import { Dogs } from "../data/dogs";
import Pet from "../components/Pet.vue";

export default {
  components: {
    appPet: Pet
  },

  data() {
    return {
      dogs: Dogs
    };
  }
};
</script>

<style scoped>
p {
  margin: 0;
}
</style>