<script setup>
import { RouterLink } from "vue-router";
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
