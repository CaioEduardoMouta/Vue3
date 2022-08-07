<template>
<div>
  <p v-if="esta_estudando">Estou estudando no momento.</p>
  <p v-else>Estou vendo novas tecnologias</p>
  <ul>
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>
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
    data() {
        return {
            esta_estudando: true,
            mostrar_email: true,
            email: "loremipsum@core.com",
            meu_link: "https://google.com"
        };
    },
   
}
</script>