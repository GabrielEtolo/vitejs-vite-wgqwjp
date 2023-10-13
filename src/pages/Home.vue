<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="px-4 py-5 my-5 text-center">
    <h1 class="display-5 fw-bold nom">Gabriel Etolo Nguini</h1>
    <h2 class="job">WebDesigner,UX/UI Designer,VueJs Develloper</h2>
    <div class="col-lg-6 mx-auto texte">
      <p class="lead mb-4">
        Bienvenue dans l'univers captivant de la conception web et du
        développement front-end en compagnie d'un passionné. Fort de ma
        formation en design web et animé par une curiosité sans limites, mon
        objectif est de créer des interfaces intuitives et esthétiques pour
        satisfaire les besoins des utilisateurs. Je vous invite chaleureusement
        à me rejoindre dans cette aventure palpitante où la créativité se marie
        harmonieusement avec la technologie pour façonner l'avenir du web.
      </p>
      <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
        <RouterLink to="/portfolio" class="btn btn-primary btn-lg px-4 gap-3"
          >Voir mon portfolio</RouterLink
        >
        <RouterLink to="/contact" class="btn btn-outline-secondary btn-lg px-4"
          >Me contacter</RouterLink
        >
      </div>
    </div>
  </div>
</template>
