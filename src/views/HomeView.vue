<script setup>
import CarrouselComponent from '../components/CarrouselComponent.vue';
import AboutComponent from '../components/AboutComponent.vue';
import ProjetsComponent from '../components/ProjetsComponent.vue';
import ExperiencesComponent from '../components/ExperiencesComponent.vue';
import EtudesComponent from '../components/EtudesComponent.vue';
import ContacterComponent from '../components/ContacterComponent.vue';
import NavigationComponent from '../components/NavigationComponent.vue';
import FooterComponent from '../components/FooterComponent.vue';
</script>

<!-- Ajouter technologies, contact et formations (certifications) -->

<template>
  <NavigationComponent />
  <ul>
    <li>
      <CarrouselComponent id="home" />
    </li>
    <li>
      <AboutComponent id="a-propos" />
    </li>
    <li>
      <ProjetsComponent id="projets" />
    </li>
    <li>
      <ExperiencesComponent id="experiences" />
    </li>
    <li>
      <EtudesComponent id="etudes" />
    </li>
    <li>
      <ContacterComponent id="contact" />
    </li>
  </ul>
  <FooterComponent />
</template>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  flex-direction: column;
  width: 100%;
}

ul li {
  margin-bottom: 7.5rem;
}

html {
  scroll-behavior: smooth;
}
</style>
