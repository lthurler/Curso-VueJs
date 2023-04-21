<template>
    <h1>Componente {{ nome }}</h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome:'Lifecycle'
        }
    },
    created() {
        setTimeout(() => {
            this.nome = 'Mudei'
        }, 1000);

        this.lifeCycle()
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'Mudei'
        }, 1000);
        this.nome = 'De novo'
    },

    methods: {
        lifeCycle() {
            console.log("executou")
        }
    }
}
</script>