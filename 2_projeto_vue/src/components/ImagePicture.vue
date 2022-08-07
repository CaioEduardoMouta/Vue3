<template>
    <div>
    <img :src="avatar" :alt="descricao">
    <ReutilizacaoReusable />
    </div>
</template>

<script>
import ReutilizacaoReusable from './ReutilizacaoReusable.vue'
export default {
    name: "PictureImage",
    data() {
        return {
            avatar: "/img/java.png",
            descricao: "Lorem Ipsum"
        };
    },
    components: { ReutilizacaoReusable }
}
</script>