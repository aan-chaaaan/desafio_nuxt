<template>
<v-app app>
      <v-flex d-flex>
      <v-layout wrap>
        <v-flex
          md4 
        >
        
          <v-card  v-for="(personaje, index) in $store.state.personajes.data"
          :key="index" class="container ma-4">
            <v-img height="350" :src='personaje.imagen'></v-img>
            <v-card-title>{{ personaje.nombre }}</v-card-title>
          </v-card>
        
        </v-flex>
      </v-layout>
    </v-flex>
  </v-app>
</template>
<script>
  export default {
    name: "Cards",
    data: () => ({
      
    }),
  }
</script>
<style>
</style>