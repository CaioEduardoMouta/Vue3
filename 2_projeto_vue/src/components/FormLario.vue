<template>
<div>
    <h2>Meu Formulário</h2>
    <form action="">
        <div>
            <InputText />
        </div>
        <div>
            <InputText />
        </div>
        <div>
            <SubMit />
        </div>
    </form>
</div>
</template>
<script>
import InputText from './form/InputText.vue';
import SubMit from './form/SubMit.vue';



    export default {
        name: 'FormLario',
        components: {
            InputText,
            SubMit
        }
    }
</script>