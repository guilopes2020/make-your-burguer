<template>
    <form action="" @submit="enviarFormulario($event)">
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <input type="email" v-model="email">
        </div>
        <submit />
    </form>
</template>

<script>
import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'
    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        },
        data() {
            return {
                name: '',
                email: ''
            }
        },
        methods: {
            enviarFormulario(e) {
                e.preventDefault();
                const name = this.name
                const email = this.email
                alert(`o nome é${name}, e o email é ${email}`)
            }
        }
    }
</script>

<style>

</style>