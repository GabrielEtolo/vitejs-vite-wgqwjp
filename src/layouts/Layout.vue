<script setup>
import { RouterLink } from "vue-router";
document.documentElement.classList.add("preparation");
window.onload = function () {
  document.documentElement.classList.remove("preparation");
  window.onload = function () {
    document.documentElement.classList.add("show-time");
  };
};
</script>

<template>
  <div class="d-flex flex-column">
    <RouterLink to="/"><header>G.E.N</header></RouterLink>
    <main class="flex-shrink-0 pb-5">
      <div class="container">
        <slot />
      </div>
    </main>
  </div>
</template>
