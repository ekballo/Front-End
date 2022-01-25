<template>
    <div>
        <p>Componente de Menssagem</p>
    </div>
    <div>
        <form id="burger-form">
            <div class="id-container">
                <label for="nome">Nome do Cliente</label>
                <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu Nome">
            </div><!--id-container-->
            <div class="id-container">
                <label for="pao">Escolha o pão:</label>
                <select name="pao" id="pao" v-model="pao">
                    <option value="">Selecione o seu pão</option>
                    <option value="">Integral</option>
                </select>
            </div><!--id-container-->
        </form><!--burger-form-->
    </div>
</template>

<script>


export default {
    name: "BurgerForm"
}
</script>

<style scoped>

</style>