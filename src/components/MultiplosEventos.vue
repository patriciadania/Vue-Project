<template>
  <div>
    <button
      @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro($event)"
    >
      Ativar múltiplos eventos
    </button>
    <p>{{ multiplos_eventos }}</p>
  </div>
</template>

<script>
export default {
  name: "MultiplosEventos",
  data() {
    return {
      multiplos_eventos: "",
      txt1: "Primeiro evento",
      txt2: "Segundo Evento",
    };
  },
  methods: {
    primeiro(txt1) {
      this.multiplos_eventos = txt1;
    },
    segundo(txt2) {
      setTimeout(() => (this.multiplos_eventos = txt2), 500);
    },
    terceiro() {
      setTimeout(() => (this.multiplos_eventos = ""), 1500);
    },
  },
};
</script>

<style scoped>
div {
  margin: 100px;
}
</style>
