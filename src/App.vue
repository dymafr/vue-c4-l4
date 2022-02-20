<template>
  <h1>Compteur : {{ compteur }}</h1>
  <button @click="incCompteur">+1</button>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const compteur = ref(0);

function incCompteur() {
  compteur.value++;
}
</script>

<style></style>
