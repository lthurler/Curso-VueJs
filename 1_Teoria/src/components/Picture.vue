<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarFoto @mudar-imagem="trocarImagem" />        
    </div>
</template>

<script>
import MudarFoto from './MudarFoto.vue';
import ReUtilizacao from './ReUtilizacao.vue';

export default {
    name: 'Picture',

    components: {
        ReUtilizacao,
        MudarFoto
    },

    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Avatar"
        }
    },

    methods: {
        trocarImagem() {
            this.avatar = "/img/avatar2.png"
        }
    }
}
</script>
