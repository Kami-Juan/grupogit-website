<template>
  <div id="container">
    <SeccionViewInicio class="section"/>
    <SeccionViewNosotros class="section"/>
    <SeccionViewEmpresas class="section"/>
    <SeccionViewContacto class="section"/>
  </div>
</template>

<script>
import $ from "jquery";
import "jquery-scrollify";

import SeccionViewInicio from "./../components/core/landing-page/SeccionViewInicio";
import SeccionViewNosotros from "./../components/core/landing-page/SeccionViewNosotros";
import SeccionViewEmpresas from "./../components/core/landing-page/SeccionViewEmpresas";
import SeccionViewContacto from "./../components/core/landing-page/SeccionViewContacto";

export default {
  name: "home",
  components: {
    SeccionViewInicio,
    SeccionViewNosotros,
    SeccionViewEmpresas,
    SeccionViewContacto
  },
  data() {
    return {};
  },
  methods: {},
  mounted() {
    $.scrollify({
      section: ".section"
    });
  },
  destroyed() {
    $.scrollify.destroy();
  }
};
</script>
