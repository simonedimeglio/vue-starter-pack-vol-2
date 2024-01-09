<!-- VEDI EMIT.MD -->
<template>
  <div>
    <ChildComponent @eventoPersonalizzato="gestisciEvento" />
    <p>{{ messaggio }}</p>
  </div>
</template>

<script>
import ChildComponent from "./EmitChild.vue";

export default {
  components: {
    ChildComponent
  },
  data() {
    return {
      messaggio: "Nessun Evento Eseguito"
    };
  },
  methods: {
    gestisciEvento(datiOpzionali) {
      // Gestisce l'evento ricevuto dal componente figlio
      this.messaggio = "Evento Eseguito con Dati: " + datiOpzionali;
    }
  }
};
</script>
