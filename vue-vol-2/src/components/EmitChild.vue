<!-- VEDI EMIT.MD -->
<template>
  <button @click="emettiEvento">Clicca per Emettere l'Evento</button>
</template>

<script>
export default {
  methods: {
    emettiEvento() {
      // Emette un evento personalizzato chiamato "eventoPersonalizzato"
      this.$emit('eventoPersonalizzato', 'Dati Opzionali');
    }
  }
};
</script>
