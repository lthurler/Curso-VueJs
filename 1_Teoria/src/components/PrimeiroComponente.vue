<template>
    <div>
        <ReUtilizacao />
        <h1>Primeiro componete</h1>
        <p>Meu nome é {{ nome }} e trabalho com {{ profissao }}</p>
        <MultiplosEventos />
        <ReUtilizacao />
        <ReUtilizacao />
        <ReUtilizacao />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import ReUtilizacao from './ReUtilizacao.vue'
    export default {
    name: 'PrimeiroComponente',

    components: {
        MultiplosEventos,
        ReUtilizacao
    },

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