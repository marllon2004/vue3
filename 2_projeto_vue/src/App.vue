<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <p>O dado de app é: {{ testando }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'

  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Header
    },
    data() {
      return {
        testando: "Teste"
      }
    }
  }
</script>

<style>
  body {
    background-color: #333;
    color: #FFF
  }
</style>