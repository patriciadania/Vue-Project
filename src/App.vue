<template>
  <div>
  <PrimeiroComponenteVue/>
  <p>O dado de app é: {{  testando }}</p>
  <LifeCycle/>
</div>
</template>

<script>
import PrimeiroComponenteVue from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue';

export default{
  name: 'App',
  components: {
    PrimeiroComponenteVue,
    LifeCycle
  },
  data(){
    return {
      testando: "Teste"
    }
  }
}
</script>