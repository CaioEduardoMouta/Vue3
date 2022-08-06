<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info />
        <Form />
    </div>
</template> 


<script>
import Info from './InforMacao.vue'
import Form from './FormLario.vue'


    export default {
        
        name: 'PessoaPerson',
        components: {
            Info,
            Form
    },
        data() {
            return {
                nome: 'Caio'
            }
        }
    }
</script>
