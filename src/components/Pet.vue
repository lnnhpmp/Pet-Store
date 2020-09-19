<template>
  <v-card color="grey lighten-2">
    <v-img :src="pet.img" height="170px"></v-img>
    <v-card-title>
      <div>
        <h3>{{pet.name}}</h3>
        <p>{{pet.breed}}</p>
      </div>
    </v-card-title>
  </v-card>
</template>

<script>
export default {
  props: {
    pet: {
      type: Object
    }
  }
};
</script>

<style>
</style>

