<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default {
    name: 'PictureImage',
    data() {
        return {
            avatar: "/img/java.png",
            descricao: "Lorem Ipsum"
        }
    }
}
</script>