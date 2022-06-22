<template>
    <div>
        <h1>Olá vue</h1>
        <p>Meu nome é {{nome}}</p>
        <MultiplosEventos/>
        <ReutilizacaoVue/>
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'
    import ReutilizacaoVue from './Reutilizacao.vue'

    export default {
        name:"PrimeiroComponente",
        components: {
            MultiplosEventos,
            ReutilizacaoVue
        },
        data(){
            return{
                nome: "Enzo",
                profissao: "programador"
            }
        }
    }
</script>