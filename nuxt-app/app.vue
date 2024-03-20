<template>
  <NavBar :routes="routes" />
  <section>
    <NuxtPage />
  </section>
</template>

<script setup lang="ts">
const routes = {
  layer1: "/layer1",
  layer2: "/layer2",
};
</script>