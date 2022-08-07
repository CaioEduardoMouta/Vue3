<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
    <PessoaPerson />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'

import PessoaPerson from './components/PessoaPerson.vue'

export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    PessoaPerson
}
}
</script>