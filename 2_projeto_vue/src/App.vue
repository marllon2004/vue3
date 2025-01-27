<template>
  <div>
    <PrimeiroComponente />
    <p>O dado de app é: {{ testando }}</p>
    <LifeCycle />
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'

  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle
    },
    data() {
      return {
        testando: "Teste"
      }
    }
  }
</script>
