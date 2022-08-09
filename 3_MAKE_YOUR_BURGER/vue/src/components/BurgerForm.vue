<template>
    <div>
    <p>Componente de Mensagem</p>
    <div>
        <form id="burguer-form">
            <div class="input-container">
                <label for="nome">Nome do cliente:</label>
                <input type="text" id="nome" name="name" v-model="nome" placeholder="digite seu nome">
            </div>
            <div class="input-container">
                <label for="pao">Escolha o pão</label>
                <select name="pao" id="pao" v-model="pao">
                    <option value="">Selecione o seu pão</option>
                    <option value="integral">Integral</option>
                </select>
                
            </div>
             <div class="input-container">
                <label for="carne">Escolha a carne do seu burguer</label>
                <select name="carne" id="carne" v-model="carne">
                    <option value="">Selecione o seu pão</option>
                    <option value="integral">Integral</option>
                </select>
                
            </div>
        </form>
    </div>
    </div>
</template>
<script>
    export default {
        name: "BurgerForm"
    }

</script>

<style >

</style>