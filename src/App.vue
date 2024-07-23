<template>
  <div>
  <PrimeiroComponenteVue/>
  <p>O dado de app é: {{  testando }}</p>
  <LifeCycle/>
  <Pessoa/>
</div>
</template>

<script>
import PrimeiroComponenteVue from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

export default{
  name: 'App',
  components: {
    PrimeiroComponenteVue,
    LifeCycle, 
    Pessoa
  },
  data(){
    return {
      testando: "Teste"
    }
  }
}
</script>