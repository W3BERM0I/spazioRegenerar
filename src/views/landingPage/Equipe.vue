<template>
  <v-container class="containerEquipe">
    <v-row class="justify-center ma-0">
      <h1 class="tituloEquipe">Nossa equipe</h1>
    </v-row>
    <v-row justify="space-evenly" v-if="profiles">
      <CardProfile
        v-for="(profile, index) in profiles"
        :key="index"
        :profile="profile"
      />
    </v-row>
  </v-container>
</template>

<script setup>
import CardProfile from "@/components/CardProfile.vue";

import { reactive } from "vue";

components: {
  CardProfile;
}

const profiles = reactive([
  {
    name: "Jani Machado",
    description:
      "Profissional especializado em massagem terapêutica e Reiki, promovendo bem-estar físico e mental através do toque terapêutico e da energia vital universal.",
    color: "var(--azulFraco)",
    imgSrc: "src/assets/jani.jpeg",
    whats: "https://wa.me/5554999145938",
    insta: "https://www.instagram.com/machado_janini2023",
  },
  {
    name: "Raquel Dall Agnol",
    description:
      "Designer de cílios especializado em criar e realçar a beleza dos olhos, utilizando técnicas avançadas e materiais de qualidade para proporcionar cílios incríveis e personalizados.",
    color: "var(--roxoFraco)",
    imgSrc: "src/assets/raquel.jpeg",
    whats: "https://wa.me/5554991588576",
    insta: "https://www.instagram.com/raqueldall_lashdesigner",
  },
]);
</script>

<style lang="scss" scoped>
.tituloEquipe {
  font-weight: 700;
  font-size: 4rem;
  margin: 40px;
}

.containerEquipe {
  min-height: 60vh;
  margin-bottom: 40px;
}
</style>