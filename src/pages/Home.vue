<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="container col-xxl-8 px-4 py-5">
    <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
      <div class="col-10 col-sm-8 col-lg-6 texte">
        <img
          src="../assets/giphy.gif"
          class="d-block mx-lg-auto img-fluid"
          alt="Bootstrap Themes"
          width=auto
          min-height= 300px
          loading="lazy"
        />
      </div>
      <div class="col-lg-6 image">
        <h1 class="display-5 fw-bold lh-1 mb-3">Gabriel Etolo Nguini</h1>
        <p class="lead">
          <h2>WebDesigner,UX/UI Designer,VueJs Develloper</h2>
          Plongez dans l'univers de la conception web et du développement front-end avec un 
          professionnel passionné : moi, un Web Designer, UX/UI Designer et développeur Vue. 
          Formé en Design web et guidé par une curiosité insatiable, je suis déterminé à créer 
          des interfaces intuitives et esthétiques pour répondre aux besoins des utilisateurs. 
          Rejoignez-moi dans cette aventure passionnante où la créativité et la technologie se 
          rejoignent pour façonner l'avenir du web.
        </p>
        <div class="d-grid gap-2 d-md-flex justify-content-md-start">
           <RouterLink to="/portfolio" class="btn btn-primary">Voir mon portfolio</RouterLink>
          <RouterLink to="/contact" class="btn btn-outline-secondary">Me contacter</RouterLink>
           

         
        </div>
      </div>
    </div>
  </div>
</template>
