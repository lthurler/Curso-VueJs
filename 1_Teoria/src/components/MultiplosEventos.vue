<template>
    <div>
        <button @click="primeiro('primeiro evento',$event), segundo('segundo evento',$event), terceiro('',$event)">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
export default {
    name:'MultiplosEventos',

    data() {
        return {
            multiplos_eventos: ""
        }
    },

    methods: {
        primeiro(txt,e) {
            this.multiplos_eventos = txt;
        },

        segundo(txt,e) {
           setTimeout(() => this.multiplos_eventos = txt, 500) 
        },

        terceiro(txt, e) {
            setTimeout(() => this.multiplos_eventos = txt, 1500)
        }
    }
}
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>
