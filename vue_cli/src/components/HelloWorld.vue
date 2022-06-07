<template>
    <div>
        <h1> Meu nome é : {{nome}}</h1>
    </div>
</template>

<script>
export default {
    name : 'HelloWorld',
    data() {
       return{
            nome: 'ainda não sei'
       } 
    },
    created() { // cria um dado
        this.nome =  "Enzo Gama"      
    },
    mounted() { // uma hierarquia acima do created
        this.nome = "Fulano de tal"
    },
    created() { // cria um dado e seta no final
        setTimeout(() => {
            this.nome =  "ciclano"
        }, 1000);
    },
}
</script>
