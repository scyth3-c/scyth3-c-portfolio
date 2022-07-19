<template>
  <b-card class="w-100 footer-vw" type="dark">
    <hr class="bg-dark" />
    <ul class="float-left mt-3 footer-list">
      <li><b-icon icon="code"></b-icon> Kevin Bohorquez</li>
      <br />
      <li><b-icon icon="github"></b-icon> scyth3-c</li>
      <li><b-icon icon="twitter"></b-icon> scyth3_c</li>
    </ul>

    <b-card no-body class="col-md-4 float-center mx-auto footer-vw">
      <strong class="text-white">scyth3-c</strong>
    </b-card>
    <hr class="bg-dark" />
  </b-card>
</template>

<script>

export default {
  name: "footerVue",
};
</script>

<style scoped>
.footer-vw {
  background: rgb(27, 27, 27);
}
.footer-list {
  list-style: none;
  color: white;
}
.text {
  font-family: "Courier New", Courier, monospace;
}
</style>