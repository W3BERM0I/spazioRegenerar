<template>
  <section class="cont">
    <carousel />
    <location />
  </section>
</template>

<script setup>
import location from "@/views/landingPage/location.vue";
import Carousel from "./landingPage/Carousel.vue";
components: {
  location;
  Carousel;
}
</script>

<style scoped>
.cont {
  background-color: var(--bege);
}
</style>
