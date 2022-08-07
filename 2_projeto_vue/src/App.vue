<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <p class="paragrafo-pai"> O dado do app é: {{ testando }}</p>
    <LifeCycle />
    <PessoaPerson />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'

import PessoaPerson from './components/PessoaPerson.vue'
import Header from './components/HeaderCabecalho.vue'

export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    PessoaPerson,
    Header
}
}
</script>

<style>
body {
  background-color: #333;
  color: #ddd;
}

a {
  color: #00FF00
}

</style>