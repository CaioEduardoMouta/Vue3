<template>
    <div>
    <h2> Esta é a descrição da Pessoa: {{ nome }}</h2>
    <Info />
    <FormLario />

    </div>
</template>
<script>
import Info from "./InforMacao.vue";
import FormLario from "./FormuLario.vue";


 export default {
    name: "PersonPeople",
    components: {
    Info,
    FormLario
},
    data() {
        return {
            nome: "Mouta"
        };
    },
    
} 
</script>