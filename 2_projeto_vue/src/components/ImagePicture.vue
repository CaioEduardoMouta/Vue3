<template>
    <div>
    <img :src="avatar" :alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue';
export default {
    name: "PictureImage",
    data() {
        return {
            avatar: "/img/java.png",
            descricao: "Lorem Ipsum"
        };
    },
    components: { MudarImagem },
    methods: {
        trocarImagem() {
            this.avatar = "/img/front.png"
        }
    }
}
</script>