<template>
  <section id="localizacao">
    <div class="loc">
      <h3>
        Venha nos visitar estamos localizados na cidade de Nova Petropolis
      </h3>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3476.862363273112!2d-51.11323078490046!3d-29.374318982131044!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x951eb3ebb53615fb%3A0xbcecb03b425ce4af!2sSpazio%20Regenerar!5e0!3m2!1spt-BR!2sbr!4v1687984685567!5m2!1spt-BR!2sbr"
        height="450"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
        class="map"
      ></iframe>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
#localizacao {
  min-height: 40vh;
  display: flex;
}

.loc {
  width: 100vw;
  height: 80vh;
  display: flex;
  justify-items: center;
  align-items: center;
}

.loc h3 {
  /*text-align: center;*/
  margin: auto 0 auto 2vw;
  font-size: 2.5rem;
  flex-wrap: wrap;
  width: 20vw;
  width: 80vw;
}

.map {
  width: 70vw;
}
</style>