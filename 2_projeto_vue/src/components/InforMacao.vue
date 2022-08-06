<template>
    <div>
        <p v-if="esta_estudando">Estou trabalhando no momento</p>
        <p>Ultilizo: </p>
        <ul>
            <li>Python</li>
            <li>PHP</li>
            <li>Java</li>
        </ul>
    </div>
</template>

<script lang="ts">
export default {
    name: 'InfoMacao',
    data() {
        return {
            esta_estudando: true
        }
    }
}

</script>
