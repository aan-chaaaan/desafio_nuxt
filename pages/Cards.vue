<template>
  <v-app app>
    <v-row>
      <v-col v-for="(personaje, index) in $store.state.personajes.data"
            :key="index" cols="12" sm="3" md="4" >
        <v-container fluid>
          <v-card
            
            class="ma-4"
          >
            <v-img height="350" :src="personaje.imagen"></v-img>
            <v-card-title>{{ personaje.nombre }}</v-card-title>
          </v-card>
        </v-container>
      </v-col>
    </v-row>
  </v-app>
</template>
<script>
export default {
  name: 'Cards',
  data: () => ({}),
}
</script>
<style></style>
