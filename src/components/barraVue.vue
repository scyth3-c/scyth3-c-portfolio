<template>
  <b-navbar toggleable="lg" class="navbar-horizontal shadow-lg">
    <b-navbar-brand>
      <b-icon icon="person-badge-fill" variant="dark"></b-icon>
      <span title="name" class="font-weight-bold mt-auto ml-3 forx"> Kevin Bohorquez Rojas</span>
    </b-navbar-brand>

    <b-navbar-nav>
      <b-nav-item href="#" class="mt-auto ml-auto">
        <b-badge variant="white">
          <span title="ocupation" class="lowtxt">Backend Engineer </span>
          <b-icon variant="secondary" icon="code-slash"></b-icon></b-badge
      ></b-nav-item>
      <b-nav-item
        href="https://goo.gl/maps/Qvpojnycmj3teTx76"
        class="mt-auto ml-auto"
      >
        <b-badge variant="white">
          <span title="location" class="lowtxt">Colombia. Bogotá, D.C </span>
          <b-icon
            variant="secondary"
            scale="0.9"
            icon="geo-alt-fill"
          ></b-icon></b-badge
      ></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto display-inline">
      <b-nav-item title="github" :href="github"
        ><b-icon icon="github" class="icon-color"></b-icon
      ></b-nav-item>
      <b-nav-item :href="mail"
        ><b-icon icon="envelope-fill" class="icon-color" ></b-icon
      ></b-nav-item>
      <b-nav-item :href="linkedin"
        ><b-icon icon="linkedin" class="icon-color" ></b-icon
      ></b-nav-item>
      <b-nav-item :href="youtube"
        ><b-icon icon="youtube" class="icon-color" ></b-icon
      ></b-nav-item>
    </b-navbar-nav>
  </b-navbar>
</template>

<script>
export default {
  name: "barraVue",
   data() {
          return {
                 github: 'https://github.com/scyth3-c',
                 mail: 'mailto:bohordo.png@gmail.com',
                 linkedin: 'https://www.linkedin.com/in/kevin-bohorquez-rojas-bohordo/',
                 youtube: 'https://www.youtube.com/channel/UCAWCJbCl07jXmPz1vHcTqWw'
          }
      }
};
</script>
<style>
.forx{
  font-family: monospace;
}
.lowtxt{
 color: rgb(58, 54, 61);
 font-weight: bolder;
}

.icon-color{
  color: black;
}

@media (max-width: 768px) {
  .icon-color{
    color: white;
  }
}

</style>