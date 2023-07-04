<template>
  <div class="header">
    <h1 style="font-family: 'Playfair Display', serif">Spazio Regenerar</h1>
    <div class="d-flex justify-center align-center navegacao">
      <p>Serviços</p>
      <p>Equipe</p>
      <p>Localização</p>
    </div>
  </div>
</template>

<script setup>
//
</script>

<style>
.header {
  position: sticky;
  top: 0;
  z-index: 1;
  display: flex;
  width: 100vw;
  justify-content: space-around;
  align-items: center;
  background-color: var(--bege);
}

.navegacao {
  display: flex;
  align-content: center;
  justify-content: space-around;
  width: 30vw;
  gap: 30px;
  font-size: 1.3rem;
}
</style>
