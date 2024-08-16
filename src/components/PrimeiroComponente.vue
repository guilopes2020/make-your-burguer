<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é: <span>{{ nome }}</span>, sou {{ profissao }} e tenho {{ idade }} anos!</p>
    <MultiploEventos />
</template>

<script>
import MultiploEventos from './MultiploEventos.vue'
    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiploEventos
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