<template>
  <!-- Un div che rappresenta il componente figlio -->
  <div class="child-component">
    <!-- Un titolo per il componente figlio -->
    <h2>Componente Figlio</h2>
    <!-- Uno slot vuoto che può essere riempito dal componente genitore -->
    <slot></slot>
  </div>
</template>

<script>
export default {
  // Nome del componente
  name: 'SlotChild'
};
</script>

<style scoped>
/* Stili CSS specifici per questo componente figlio */
  .child-component {
    border: 1px solid #ccc;
    padding: 10px;
    margin: 10px;
  }
</style>
