<template>
  <div>
    <PrimeiroCompnente />
    <p>O dado de app é: {( testando )}</p>
    <LifeCycle />
  </div>
</template>

<script>
  import PrimeiroCompnente from './components/PrimeiroCompnente.vue'
  import LifeCycle from './components/LifeCycle.vue'


  export default {
    name: 'App',
    components: {
    PrimeiroCompnente,
    LifeCycle
},
     data() {
            return {
                testando: "Teste"
            }
        }
  }
</script>
