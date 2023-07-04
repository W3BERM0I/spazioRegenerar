<template>
  <section class="cont">
    <scrollUp />
    <carousel />
    <hr />
    <Equipe />
    <hr />
    <location />
  </section>
</template>

<script setup>
import scrollUp from "@/components/scrollUp.vue";
import location from "@/views/landingPage/location.vue";
import Carousel from "./landingPage/Carousel.vue";
import Equipe from "./landingPage/Equipe.vue";

components: {
  location;
  Carousel;
  scrollUp;
  Equipe;
}
</script>

<style scoped>
.cont {
  background-color: var(--bege);
  color: var(--cinzaClaro);
}
</style>
