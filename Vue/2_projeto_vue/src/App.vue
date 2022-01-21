<template>
    <div>
      <PrimeiroComponente />
      <p>O dado de app é {{ testando }}</p>
      <LifeCycle />
    </div>
</template>


<script>
import PrimeiroComponente from'./components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'

  export default{
    nome: 'app',
    components: {
      PrimeiroComponente,
      LifeCycle
    },
    data() {
      return {
        testando: "teste"
      }
    },
  }
</script>
