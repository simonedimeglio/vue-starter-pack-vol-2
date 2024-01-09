<template>
	<!-- Utilizzo del componente Card con diverse props. -->
  <!-- Posso "hardcodare" le props o passarle dinamicamente da data() -->
	<Card titolo="Card 1" corpo="Lorem Ipsum" tema="light" />
	<Card titolo="Card 2" corpo="Ipsum Lorem" tema="light" />
	<Card :titolo="title" :corpo="main" tema="dark" />
  <br>
  <!-- VEDI EMIT.md -->
  <EmitParent />
  <!-- VEDI SLOT.md -->
  <SlotParent />
</template>

<script>
// Import dei componenti utilizzati
import Card from "./components/Card.vue";
import EmitParent from "./components/EmitParent.vue";
import SlotParent from './components/SlotParent.vue';

export default {
	// Nome del componente principale.
	name: "App",
	// Dati locali del componente principale.
	data() {
		return {
			title: "Card 3",
			main: "Sit amet",
		};
	},
	// Dichiarazione dei componenti utilizzati all'interno di questo componente.
	components: {
		Card,
    EmitParent,
    SlotParent
	},
};
</script>

<style>
/* Stili opzionali per il componente principale. */
</style>
