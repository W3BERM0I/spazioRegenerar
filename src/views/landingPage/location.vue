<template>
  <section id="localizacao">
    <div class="loc">
      <h3>
        Seja bem-vindo(a) ao nosso espaço, onde cuidamos do seu bem-estar por
        dentro e por fora. Venha nos visitar em um espaço acolhedor, onde
        combinamos serviços de massagem terapeutica e design de cílios. Nossa
        equipe experiente e qualificada está pronta para ajudar você a alcançar
        seus objetivos de saúde e beleza. Deixe-nos cuidar de você e
        proporcionar uma experiência completa de cuidados estéticos e de saúde.
        Agende sua visita hoje mesmo e dê um passo em direção à sua melhor
        versão!
      </h3>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3476.862363273112!2d-51.11323078490046!3d-29.374318982131044!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x951eb3ebb53615fb%3A0xbcecb03b425ce4af!2sSpazio%20Regenerar!5e0!3m2!1spt-BR!2sbr!4v1687984685567!5m2!1spt-BR!2sbr"
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
  height: 50vh;
  display: flex;
  justify-items: center;
  align-items: center;
}

.loc h3 {
  /*text-align: center;*/
  margin: auto 0 auto 2vw;
  font-size: 2rem;
  flex-wrap: wrap;
  width: 20vw;
  width: 80vw;
  margin-right: 10px;
  color: var(--cinzaClaro);
}

.map {
  width: 60vw;
  height: 100%;
}
</style>