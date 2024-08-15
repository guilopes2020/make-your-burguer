<template>
  <Header />
  <PrimeiroComponente />
  <LifeCycle />
  <Pessoa />
</template>

<script>
import Header from './components/Header.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue' 
  export default {
    name: 'App',
    components: {
      Header,
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Form
    }
  }
</script>

<style>
  body {
    background-color: #333;
    color: #FFF;
  }
  a{
    color: red;
  }
</style>