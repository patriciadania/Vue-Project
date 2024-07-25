<template>
  <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
  name: "LyfeCycle",
  data() {
    return {
      nome: "Ainda nao sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Matheus";
    }, 1000);
    this.lifeCycle();
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Pedro";
    }, 2000);
    this.lifeCycle();
  },
  methods: {
    lifeCycle() {
      console.log("EXECUTOU");
    },
  },
};
</script>
