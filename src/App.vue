<template>
  <h2>Prix total HT : {{ prixHT }}</h2>
  <h2>Prix total TTC : {{ prixTTC }}</h2>
</template>

<script setup lang="ts">
import { computed, reactive } from 'vue';

const produit = reactive({
  quantite: 3,
  prix: 10,
  nom: 'livre',
});

const prixHT = computed(() => produit.quantite * produit.prix);
const prixTTC = computed(() => produit.quantite * produit.prix * 1.2);
</script>

<style></style>
