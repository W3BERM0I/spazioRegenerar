<template>
  <v-bottom-navigation :elevation="5">
    <v-btn value="recent">
      <v-icon icon="md:info"></v-icon>

      Sobre
    </v-btn>

    <v-btn value="favorites">
      <v-icon>mdi-heart</v-icon>

      Serviços
    </v-btn>

    <v-btn value="nearby">
      <v-icon>mdi-map-marker</v-icon>

      Contato
    </v-btn>

    <v-btn value="nearby">
      <v-icon>mdi-map-marker</v-icon>

      Localização
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {};
</script>

<style>
</style>