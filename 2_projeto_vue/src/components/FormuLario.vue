|<template>
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
</template>

<script>
import InputText from './form/InputText.vue';
import SubMit from './form/SubMit.vue';
    
    export default {
        name: 'FormuLario',
        components: {
    InputText,
    SubMit
}
}
</script>