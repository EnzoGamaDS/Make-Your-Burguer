<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue'

export default {
    name: 'Picture',
    components: {
        MudarImagem
    },
    data() {
        return {
            avatar: "./images/avatar.png",
            descricao: "Enzo Gama"
        }
    },
    methods:{
        trocarImagem(){
            console.log("Cheguei aqui")
            this.avatar = './images/foto1.jpg'
        }
    }
}
</script>