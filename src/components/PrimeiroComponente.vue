<template>
  <div>
    <h1>OLA VUE</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos/>
    <Reutilizacao/>
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reutilizacao from './Reutilizacao.vue';

export default {
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos,
    Reutilizacao
  },
  data() {
    return {
      nome: "Patricia",
      profissao: "Desenvolvedora"
    };
  },
};
</script>
