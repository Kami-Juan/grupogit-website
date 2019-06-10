<template>
  <section>
    <div id="background"></div>
    <div class="section__title">
      <HomeSectionHeader/>
      <img :src="require('./../../../assets/img__logo.svg')" alt="grupogit">
      <h1>
        Especialistas en el desarrollo de soluciones integrales en el ramo de las
        <br>Tecnologías de la Información (TI).
      </h1>
    </div>
  </section>
</template>
<script>
import HomeSectionHeader from "./../home/HomeSectionHeader";

export default {
  components: {
    HomeSectionHeader
  }
};
</script>
<style scoped>
section {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  text-align: center;
}

#background {
  height: 100vh;
  width: 100%;
  background: linear-gradient(
      -135deg,
      rgb(0, 128, 64) 0%,
      rgb(0, 168, 156) 35%,
      rgb(22, 136, 201) 67%,
      rgb(27, 69, 128) 100%
    ),
    url(../../../assets/img__backgroud_inicio.jpg);
  display: flex;
  background-size: cover;
  opacity: 0.9;
  position: absolute;
  background-blend-mode: multiply;
  z-index: 1;
}

section img {
  max-width: 30%;
  height: 75%;
}

section h1 {
  font-size: 2em;
  margin: 0.5em 0;
  color: white;
}

section .section__title {
  width: 75%;
  margin: auto;
  z-index: 2;
}
</style>
