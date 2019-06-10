<template>
  <div class="section__navbar">
    <img :src="require('./../../../assets/img__logo_simple.svg')" alt>
    <img :src="require('./../../../assets/img__logo_menubar.svg')" alt>
    <HomeSectionScroller/>
  </div>
</template>
<script>
import HomeSectionScroller from "./HomeSectionScroller";

export default {
  components: {
    HomeSectionScroller
  }
};
</script>
<style scoped>
img {
  max-width: 30%;
  height: 75%;
}

.section__navbar {
  position: fixed;
  display: flex;
  justify-content: space-between;
  top: 0;
  left: 0;
  width: 100%;
}

.section__navbar img {
  height: 3em;
  width: 3em;
  margin: 1em 2em;
  cursor: pointer;
}

.section__navbar img:first-child {
  height: 6em;
  width: 6em;
}
</style>
