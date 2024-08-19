<template>
    <div>
        <button @click="ativar($event)">clique aqui</button>
        <span v-show="ativou">Ativado</span>
    </div>
</template>

<script>
    export default {
        name: 'Reultilizacao',
        data() {
            return {
                ativou: false
            }
        },
        methods: {
            ativar($e) {
                this.ativou = !this.ativou;
            }
        }
    }
</script>

<style>

</style>