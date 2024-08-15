<template>
    <p v-if="esta_trabalhando">estou trabalhando no momento</p>
    <p v-else>estou em busca de novas oportunidades</p>
    <p>ultilizo as seguintes tecnologias:</p>
    <ul>
        <li>PHP</li>
        <li>Mysql</li>
        <li>javascript</li>
        <li>mysql</li>
    </ul>
    <div>
        <button @click="showEmail">{{ texto_botao }}</button>
    </div>
    <p v-show="mostrar_email">mande uma mensagem para {{ email }}</p>
    <p>para acessar meu portifolio <a target="_blank" v-bind:href="meu_link">basta clicar aqui</a></p>
    <Picture></Picture>
</template>

<script>
    import Picture from './Picture.vue'
    export default {
        name: 'Info',
        data() {
            return {
                esta_trabalhando: false,
                email: 'guilopesdev@gmail.com',
                mostrar_email: false,
                texto_botao: 'Mostrar email',
                meu_link: 'https://github.com/guilopes2020/'
            }
        },
        components: {
            Picture
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if (! this.mostrar_email) {
                    this.texto_botao = 'Mostrar email'
                } else {
                    this.texto_botao = 'Esconder email'
                }
            }
        }
    }
</script>

<style scoped>

</style>