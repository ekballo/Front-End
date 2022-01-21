<template>
    <div>
      <PrimeiroComponente />
      <p>O dado de app é {{ testando }}</p>
    </div>
</template>


<script>
import PrimeiroComponente from'./components/PrimeiroComponente.vue'
  export default{
    nome: 'app',
    components: {
      PrimeiroComponente
    },
    data() {
      return {
        testando: "teste"
      }
    },
  }
</script>
