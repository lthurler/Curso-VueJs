<template>
    <h1>Primeiro componete</h1>
    <p>Meu nome é {{ nome }} e trabalho com {{ profissao }}</p>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: "Leandro",
                profissao: "Programador"
            }
        }
    }

</script>

<style scoped>

</style>