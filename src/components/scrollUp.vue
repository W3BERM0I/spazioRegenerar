<template>
  <div
    class="counterDiv d-flex justify-center align-center rounded-circle"
    v-esconder-seta-scroll
  >
    <v-icon @click.prevent="scrollUp" class="counter">mdi-chevron-up</v-icon>
  </div>
</template>

<script>
export default {
  methods: {
    scrollUp() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
  },
  computed: {
    counter() {
      return this.$store.state.counter;
    },
  },
  directives: {
    "esconder-seta-scroll": {
      bind(el) {
        window.addEventListener("scroll", () => {
          el.style.display =
            posicaoScroll >= window.scrollY > 300 ? "none" : "block";
        });
      },
    },
  },
};
</script>

<style scoped>
.counterDiv {
  position: absolute;
  bottom: 15px;
  right: 15px;
  min-width: 50px;
  min-height: 50px;
  aspect-ratio: 1/1;
  background: var(--azulFraco);
  background: linear-gradient(
    90deg,
    var(--azulFraco) 0%,
    var(--roxoFraco) 100%
  );
}

.counter {
  color: white;
  font-weight: bolder;
  font-size: 3rem;
  margin: 15px;
  cursor: pointer;
}
</style>