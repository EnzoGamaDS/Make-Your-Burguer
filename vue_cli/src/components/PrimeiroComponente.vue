<template>
    <div>
        <h1>Olá vue</h1>
        <p>Meu nome é {{nome}}</p>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                nome: "Enzo"
            }
        }
    }
</script>