<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default {
        name: 'Picture',
        data() {
            return {
                avatar: '/img/avatar.jpeg',
                descricao: 'Guilherme Lopes'
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