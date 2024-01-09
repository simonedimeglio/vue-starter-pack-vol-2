<template>
	<!-- Un div che rappresenta il componente genitore -->
	<div>
		<!-- Un titolo per il componente genitore -->
		<h1>Componente Genitore</h1>
		<!-- Utilizzo del componente figlio SlotChild -->
		<SlotChild>
			<!-- Contenuto specifico inserito nello slot del componente figlio -->
			<p>Contenuto da inserire nello slot</p>
		</SlotChild>
	</div>
</template>

<script>
// Importa il componente figlio SlotChild
import SlotChild from "./SlotChild.vue";

export default {
	// Componenti utilizzati in questo componente genitore
	components: {
		SlotChild,
	},
};
</script>
