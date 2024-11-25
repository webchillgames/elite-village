<script setup lang="ts">
import AllSections from "./src/AllSections.vue";
import SPromo from "./src/components/SPromo.vue";
</script>

<template>
  <div>
    <NuxtRouteAnnouncer />

    <SPromo />
    <!-- <NuxtWelcome /> -->
    <AllSections />
  </div>
</template>
