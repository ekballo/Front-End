<template>
    <div>
        <p>Componente de Menssagem</p>
    </div>
    <div>
        <form id="burger-form">
            <div class="input-container">
                <label for="nome">Nome do Cliente</label>
                <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu Nome">
            </div><!--id-container-->
            <div class="input-container">
                <label for="pao">Escolha o pão:</label>
                <select name="pao" id="pao" v-model="pao">
                    <option value="">Selecione o seu pão</option>
                    <option value="integral">Integral</option>
                </select>
            </div><!--id-container-->
            <div class="input-container">
                <label for="carne">Escolha a carne do seu Burger:</label>
                <select name="carne" id="carne" v-model="carne">
                    <option value="">Selecione o tipo de carne</option>
                    <option value="contra-file">Contra-Filé</option>
                </select>
            </div><!--id-container-->
            <div id="opcionais-container" class="input-container">
                <label id="opcionais-title" for="opcionais">Escolha os Opcionais:</label>
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div><!--checkbox-container-->
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div><!--checkbox-container-->
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div><!--checkbox-container-->
            </div><!--id-container-->
            <div class="input-container">
                <input type="submit" class="submit-btn" value="Criar meu Burger">
            </div>
        </form><!--burger-form-->
    </div>
</template>

<script>


export default {
    name: "BurgerForm"
}
</script>

<style scoped>
    #burger-form{
        max-width: 400px;
        margin: 0 auto;
    }
    .input-container{
        display: flex;
        flex-direction: column;
        margin-bottom: 20px;
    }

    label{
        font-weight: bold;
        margin-bottom: 15px;
        color: #222;
        padding: 5px 10px;
        border-left: 4px solid #FCBA03;
    }

    input, select {
        padding: 5px 10px;
        width: 300px;
    }

    #opcionais-container{
        flex-direction: row;
        flex-wrap: wrap;
    }

    #opcionais-title {
        width: 100%;
    }
    .checkbox-container{
        display: flex;
        align-items: flex-start;
        width: 50%;
        margin-bottom: 20px;
    }
</style>