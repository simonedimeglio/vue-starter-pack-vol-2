<!-- VEDI PROPS.MD -->
<template>
	<!-- Il componente Card rappresenta una card con un titolo, un corpo e uno stile opzionale. -->
	<div class="card" :class="{ dark: tema === 'dark' }">
		<!-- Titolo della card -->
		<h1>{{ titolo }}</h1>
		<!-- Testo della card -->
		<p>{{ corpo }}</p>
	</div>
</template>

<script>
export default {
	// Definizione delle props necessarie per il componente Card.
	props: ["titolo", "corpo", "tema"],
};
</script>

<style>
/* Stili per il componente Card. */
.card {
	border: 1px solid #ccc;
	background-color: #fff;
	color: rgb(59, 59, 59);
	text-align: center;
	border-radius: 12px;
	width: 400px;
	height: 400px;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}
/* Stile aggiuntivo se il tema è impostato su 'dark'. */
.dark {
	background-color: #333;
	color: #fff;
}
</style>
