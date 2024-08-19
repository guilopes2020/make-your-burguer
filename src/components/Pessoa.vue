<template>
    <h2>esta é a descrição da pessoa: <span>{{ nome }}</span></h2>
    <Info :email="email" :esta_trabalhando="false" />
    <Form></Form>
</template>

<script>
import Info from './Info.vue'
import Form from './Form.vue'
    export default {
        name: 'Pessoa',
        data() {
            return {
                nome: 'Gregregreg',
                email: 'gregreg@gmail.com',
            }
        },
        components: {
            Info,
            Form
        }
    }
</script>

<style scoped>
    h2 {
        color: blueviolet;
    }
    span {
        color: yellowgreen;
    }
</style>