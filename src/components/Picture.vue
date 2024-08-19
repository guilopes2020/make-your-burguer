<template>
    <img :src="avatar" :alt="descricao">
    <MudarImagem @mudar-imagem="MudarImagem" />
</template>

<script>
import MudarImagem from './MudarImagem.vue'
    export default {
  components: { MudarImagem },
        name: 'Picture',
        data() {
            return {
                avatar: '/img/avatar.jpeg',
                descricao: 'Guilherme Lopes'
            }
        },
        methods: {
            MudarImagem() {

                // this.avatar = '/img/burger.jpg'

                if (this.avatar != '/img/avatar.jpeg') {
                    this.avatar = '/img/avatar.jpeg'
                } else {
                    this.avatar = '/img/burger.jpg'
                }
            }
        }
    }
</script>

<style scoped>
    img {
        width: 200px;
        height: 200px;
        border-radius: 100%;
        box-shadow: 10px 10px 10px black;
        transition: 0.5s;
    }
    img:hover {
        scale: 1.1;
        box-shadow: 0px 0px 10px blue;
    }
</style>