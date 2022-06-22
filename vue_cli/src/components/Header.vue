<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
        <li v-if="estaLogado">Meu perfil</li>
    </ul>

</template>

<script>
export default {
    name: 'Header',
    props:["estaLogado"]
}
</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background: #999;
    }
    li{
        margin-right: 10px;
    }
    a{
        color: #ddd;
        transition: .5s;
    }
    a:hover{
        color: turquoise;
    }
</style>