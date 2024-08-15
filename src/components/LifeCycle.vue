<template>
    <h1>meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'ainda nao sei'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Matheus'
            }, 1000)
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 2000)
        }
    }
</script>

<style scoped>

</style>