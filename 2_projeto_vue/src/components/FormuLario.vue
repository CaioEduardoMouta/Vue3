|<template>
    <form action="" @submit="enviarFormulario($event)">
        <div>
        <input type="text" v-model="name" />
        </div>
        <div>
        <input type="text" v-model="email" />
        </div>
        <div>
        <SubMit />
        </div>
    </form>
    <p>Conteúdo</p>
</template>

<script>

import SubMit from './form/SubMit.vue';
    
    export default {
        name: 'FormuLario',
        components: {
        SubMit
    },
    data() {
        return {
            name: "",
            email: ""
        }
    },
    methods: {
        enviarFormulario(e) {

            e.preventDefault();

            const name = this.name;
            const email = this.email;

            console.log("formulario enviado")
            console.log("O nome é: " + name);
            console.log("O email é: " + email);


        }
    }
}
</script>

<style scoped>
    p {
        margin:150px;
    }
</style>