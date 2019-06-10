<template>
  <section class="section__info">
    <div class="section__nosotros container">
      <h2>Nuestros Servicios</h2>
      <h3>
        Con firme conocimiento del campo tecnológico actual, ofrecemos la siguiente
        <br>gama de servicios:
      </h3>
      <div class="row">
        <figure class="col-md-4" v-for="(info, i) in list_info_nosotros" :key="i">
          <img :src="info.url" alt>
          <figcaption>
            <h3 v-html="info.title"></h3>
            <p v-html="info.content"></p>
          </figcaption>
        </figure>
      </div>
    </div>
    <div class="section__carousel"></div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      list_info_nosotros: [
        {
          title: "Consultoría en Desarrollo de <br/> Software",
          content:
            "Analizamos y diseñamos una propuesta de solución acorde a los objetivos y requerimientos de cada proyecto, con la finalidad de dimensionar el alcance y los recursos necesarios para su desarrollo.",
          url: require("./../../../assets/img__logo_info.svg")
        },
        {
          title: "Desarrollo de <br/> Software",
          content:
            "Construimos plataformas tecnológicas de primer nivel: interfaces de comunicación, sistemas de escritorio, aplicaciones web y móviles.",
          url: require("./../../../assets/img__logo_info_fabrica.svg")
        },
        {
          title: "Outsourcing Desarrollo de <br> Software",
          content:
            "Creamos equipos de trabajo acorde a las necesidades de los clientes. La experiencia de nuestros ingenieros radica en la amplia gama de proyectos implementados para diversos sectores empresariales.",
          url: require("./../../../assets/img_logo_info_outsourcing.svg")
        }
      ]
    };
  }
};
</script>
<style scoped>
@font-face {
  font-family: "AvenirBold";
  src: url(../../../assets/AvenirLTStd-Bold.ttf);
}

.section__info h2 {
  font-size: 36px;
  margin: 0;
}

.section__nosotros > h3 {
  font-size: 24px;
  margin: 16px 0 36px 0;
}

.section__nosotros p {
  font-size: 16px;
}

.section__info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  text-align: center;
  color: white;
  font-family: "AvenirBold";
}
</style>
