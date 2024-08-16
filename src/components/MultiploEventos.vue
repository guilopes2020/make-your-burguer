<template>
    <div>
        <button @click="primeiro(priEvent, $event), segundo(secondEvent, $event), terceiro(limpar, $event)">ativar multiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiploEventos',
        data() {
            return {
                multiplos_eventos: '',
                priEvent: 'primeiro evento ativado',
                secondEvent: 'segundo evento ativado',
                limpar: ''
            }
        },
        methods: {
            primeiro(priEvent, e) {
                this.multiplos_eventos = priEvent
            },
            segundo(secondEvent, e) {
                setTimeout(() => {
                    this.multiplos_eventos = secondEvent
                }, 1000)
            },
            terceiro(limpar, e) {
                setTimeout(() => {
                    this.multiplos_eventos = limpar
                }, 2000)
            }
        }
    }
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>