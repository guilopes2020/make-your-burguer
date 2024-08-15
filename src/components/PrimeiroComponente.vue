<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é: <span>{{ nome }}</span>, sou {{ profissao }} e tenho {{ idade }} anos!</p>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
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