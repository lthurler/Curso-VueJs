<template>
    <div>
        <h2>Meu formulário:</h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <InputText />
            </div>
            <div>
                <InputText />
            </div>
            <div>
                <Submit />
            </div>
        </form>
        <p>Conteúdo</p>
        <p>Conteúdo</p>
        <p>Conteúdo</p>
    </div>
</template>

<script>
import InputText from "./InputText.vue"
import Submit from "./Submit.vue"
export default {
    name: 'Form',
    components: {
        InputText,
        Submit
    },

    methods: {
        enviarFormulario(e) {

            e.preventDefault();

            console.log("Formulario de enviado!");
        }
    }
}
</script>

<style scoped>
    p {
        margin: 150px;
    }
</style>