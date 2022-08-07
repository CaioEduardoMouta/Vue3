<template>
<div>
  
  <p v-if="esta_estudando">Estou estudando no momento.</p>
  <p v-else>Estou vendo novas tecnologias</p>
  <p>Ultilizo as seguintes tecnologias para back-end</p>
  <ul>
    <li v-for="(technology, index) in backend_technologies" v-bind:key="index">{{ technology }}</li>  
  </ul>

  <p>Utilizo as seguintes tecnologias para front-end</p>
  <ul>
    <li v-for="technology in frontend_technologies" :key="technology.id">
        {{ technology.language }}
    </li>
  </ul>
  <div>
    <button @click="showEmail">{{ textoBotao }}</button>
  </div>
  <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
  <p>Para acessar meu portfólio <a v-bind:href="meu_link">basta clicar aqui</a></p>
  <Picture />
</div>
</template>
<script>
import Picture from './ImagePicture.vue'
export default {
    name: "InforMacao",
    components: { Picture },
    props: {
        email: String,
        esta_estudando: Boolean
    },
    data() {
        return {
            mostrar_email: false,
            meu_link: "https://google.com",
            textoBotao: 'Mostrar e-mail',
            backend_technologies: ['JS', 'Java', 'Python'],
            frontend_technologies: [
                {id:1, language:'HTML'}, 
                {id:2, language:'CSS'},
                {id:3, language:'Vue'}
            ]
        }
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Esconder e-mail'
            }
        }
    }
   
}
</script>
<style>
    .paragrafo-pai {
        color: red;
    }
</style>