<template>
  <div>
    <PrimeiroCompnente />
    <p>O dado de app é: {( testando )}</p>
    <LifeCycle />
    <Pessoa />
   
  </div>
</template>

<script>
  import PrimeiroCompnente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/PessoaPerson.vue'
 

  export default {
    name: 'App',
    components: {
      PrimeiroCompnente,
      LifeCycle,
      Pessoa  
},
     data() {
            return {
                testando: "Teste"
            }
        }
  }
</script>
