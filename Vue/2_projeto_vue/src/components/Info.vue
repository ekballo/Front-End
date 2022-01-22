<template>
  <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades!</p>
  <p>Utilizo as seguintes tecnologias:</p>
  <ul>
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>
</template>
<script>
export default {
  name: 'Info',
  data() {
    return { 
      esta_trabalhando: true
    }
  }
}
</script>