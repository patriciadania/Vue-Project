<template>
  <div>
    <h1>OLA VUE</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos/>
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';

export default {
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos
  },
  data() {
    return {
      nome: "Patricia",
      profissao: "Desenvolvedora"
    };
  },
};
</script>
