<template>
    <div>
    <h2> Esta é a descrição da Pessoa: {{ nome }}</h2>
    <Info :email="email" esta_estudando: true />
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
            nome: "Mouta",
            email: "mouta@email.com"
        }
    }
    
} 
</script>