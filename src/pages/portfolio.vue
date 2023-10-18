<template>
  <div class="folio">
    <div class="one"></div>
    <div class="five"></div>
    <div class="two"></div>

    <button class="three" onclick="Show('threepush')" />
    <button class="four" onclick="Show('fourpush')" />
  </div>
  <div id="fourpush">
    <button class="quit" onclick="hide('fourpush')">X</button>
    <h1><b>Insamui</b></h1>

    <div class="project">
      <section class="gallery">
        <img
          id="myImg"
          src="../../public/img/p1bck.png"
          alt="img"
          style="max-width: 400px"
        />
      </section>
      <section class="texte">
        <h2>Entreprise de Gestion Locatives</h2>

        Le site "Insamui" pour une agence de gestion locative en Thaïlande,
        dédiée à Koh Samui, présente une interface moderne et conviviale. Il
        facilite la recherche de biens immobiliers en mettant en avant des
        propriétés variées et des paysages exotiques. Le site offre également
        des informations détaillées sur les services de gestion locative, tout
        en renforçant la confiance des visiteurs par le biais de témoignages
        clients et de guides pratiques. L'objectif est de positionner "Insamui"
        comme une agence de confiance dans le secteur de la gestion locative en
        Thaïlande.
        <br />
        <RouterLink to="/contact">Me contacter</RouterLink>
      </section>
    </div>
    <div class="skills">
      <div class="texte">
        <a
          href="https://www.figma.com/file/FTDG7BKBp8iiJe4A1SwWIs/Untitled?type=design&node-id=94-16&mode=design&t=BbLvk5yiDaggKqqU-0"
        >
          <img src="../../public/img/fig.png" alt="img" />
          Template et design créé sur figma
        </a>
      </div>

      <div class="texte">
        <a href="https://gen-portfolio-six.vercel.app/">
          <img src="../../public/img/vue.png" alt="img" />
          Site dévelloper et déployé avec VueJs 3</a
        >
      </div>
    </div>
  </div>
  <div id="threepush">
    <button class="quit" onclick="hide('threepush')">X</button>
    <h1><b>Festival des Djinns</b></h1>

    <div class="project">
      <section class="gallery">
        <img
          id="myImg"
          src="../../public/img/p1bck.png"
          alt="img"
          style="max-width: 400px"
        />
      </section>
      <section class="texte">
        <h2>Réalisation de menu à cocktail</h2>
        Madame, Monsieur, Je vous présente mon dernier projet : des cartes de
        cocktails illustrées dans un style de bande dessinée. Elles répertorient
        les ingrédients et capturent l'essence de chaque boisson. Mon objectif
        est de raviver la passion des amateurs de cocktails et de les aider à se
        souvenir des recettes tout en évoquant les émotions associées. J'espère
        que ce projet vous inspirera. Cordialement, GEN
        <br />
        <RouterLink to="/contact">Me contacter</RouterLink>
      </section>
    </div>
    <div class="skills">
      <div class="texte">
        <a
          href="https://www.figma.com/community/file/1227293216113408583/the-recette-a-cocktail"
        >
          <img src="../../public/img/figm.png" alt="img" />
          design créé sur figma
        </a>
      </div>
      <div class="texte">
        <a href="https://www.pinterest.com/lefould/">
          <img src="../../public/img/pin.png" alt="img" />
          Découvrez mon Pinterest
        </a>
      </div>
    </div>
  </div>
</template>
<script setup>
import { RouterLink } from "vue-router";
const images = [
  "../../public/img/p1bck.png",
  "../../public/img/p2bck.png",
  "../../public/img/p3bck.png",
  "../../public/img/p4bck.png",
  "../../public/img/p5bck.png",
];
const myImg = document.getElementById("myImg");
setInterval(() => {
  for (let index = 0; index++; index <= images.length - 1) {
    if (index === images.length - 1) {
      index = 0;
    } else {
      myImg.src = images[index];
    }
  }
}, 2000);
</script>
