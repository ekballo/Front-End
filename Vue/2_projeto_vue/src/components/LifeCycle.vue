<template>
    <h1>Meu Nome é: {{ nome }} </h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'Ainda não sei'
        }
    },
    created() {
        setTimeout(() =>{
            this.nome = 'Jefferson'
        }, 1000);
    },
    mounted() {
        setTimeout(() =>{
            this.nome = 'Vitoria'
        }, 2000);
    }
}
</script>
