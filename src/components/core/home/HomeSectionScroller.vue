<template>
  <div class="section__navigation">
    <ol>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
    </ol>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
ol {
  z-index: 15;
  text-align: center;
  list-style: none;
}

li {
  position: relative;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  margin-bottom: 25px;
  text-indent: -999px;
  cursor: pointer;
  opacity: 0.54;
  background: white;
  border: 1px solid #a1a1a1;
}

ol .active {
  opacity: 0.87;
  background: -webkit-linear-gradient(
    225deg,
    rgb(27, 69, 128) 0%,
    rgb(22, 136, 201) 35%,
    rgb(0, 168, 156) 67%,
    rgb(0, 128, 64) 100%
  );
  background: linear-gradient(
    -135deg,
    rgb(27, 69, 128) 0%,
    rgb(22, 136, 201) 35%,
    rgb(0, 168, 156) 67%,
    rgb(0, 128, 64) 100%
  );
}

.section__navigation {
  position: fixed;
  padding: 24px;
  right: 0;
  bottom: 0;
  top: 35%;
  z-index: 10;
}
</style>
