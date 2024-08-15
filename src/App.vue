<template>
  <PrimeiroComponente />
  <LifeCycle />
  <Pessoa />
</template>

<script>
  import LifeCycle from './components/LifeCycle.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue' 
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Form
    }
  }
</script>

<style scoped>
  
</style>