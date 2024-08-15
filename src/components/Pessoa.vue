<template>
    <h2>esta é a descrição da pessoa: <span>{{ nome }}</span></h2>
    <Info />
    <Form></Form>
</template>

<script>
import Info from './Info.vue'
import Form from './Form.vue'
    export default {
        name: 'Pessoa',
        data() {
            return {
                nome: 'Gregregreg'
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