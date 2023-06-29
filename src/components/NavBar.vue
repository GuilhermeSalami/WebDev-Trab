<template>
  <nav class="fixed-navbar">
    <v-app-bar app color="black" dark flat class="px-5">
      <v-btn>
        <v-icon color="amber-accent-3" left class="mr-3">fas fa-dragon</v-icon> Dragon's Den
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn text @click="scrollTo('inicio')" class="text-white">Início</v-btn>
      <v-btn text @click="scrollTo('sobre')">Sobre</v-btn>
      <v-btn text @click="scrollTo('portfolio')">Portfolio</v-btn>
      <v-btn text @click="scrollTo('serviços')">Serviços</v-btn>
      <v-btn text @click="scrollTo('extra')">Extra</v-btn>
      <v-btn text @click="scrollTo('contato')">Contato</v-btn>
    </v-app-bar>
  </nav>
</template>

<script>
export default {
  methods: {
    scrollTo(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: 'smooth' });
    },
  },
};
</script>

<style>
.fixed-navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 9999;
}
</style>
