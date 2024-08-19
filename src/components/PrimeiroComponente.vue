<template>
    <Reultilizacao />
    <h1>Olá Vue!</h1>
    <p>Meu nome é: <span>{{ nome }}</span>, sou {{ profissao }} e tenho {{ idade }} anos!</p>
    <MultiploEventos />
    <Reultilizacao />
    <Reultilizacao />
    <Reultilizacao />
    <Reultilizacao />
</template>

<script>
import MultiploEventos from './MultiploEventos.vue'
import Reultilizacao from './Reultilizacao.vue'
    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiploEventos,
            Reultilizacao
        },
        data() {
            return {
                nome: 'Guilherme',
                profissao: 'programador',
                idade: 42
            }
        }
    }
</script>

<style scoped>
    h1 {
        color: blue;
    }
    p {
        color: black;
    }
    span {
        color: crimson;
    }
</style>