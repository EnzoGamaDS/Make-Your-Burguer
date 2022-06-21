<template>
    <div>
        <form action="" @submit="enviarFormulario($event)">
            <div><input type="text" v-model="name"></div> 
            <div><input type="text" v-model="email"></div> 
            <div><InputTextVue/></div> 
            <input type="submit" class="button">
        </form>

        <p>Aprendendo VueJS </p>
        <p>Aprendendo VueJS </p>
        <p>Aprendendo VueJS </p>
   
    </div>    
</template>
<script>
import InputTextVue from './Form/InputText.vue'
    export default {
        components : {
            InputTextVue
        },
        data(){
            return {
                name: "Enzo",
                email:"gamaenzo@hotmail.com"
            }
        },
        methods: {
         enviarFormulario(e){
            e.preventDefault();
            const name = this.name;
            const email = this.email;
            console.log("O nome é "+name);
            console.log("O email é "+email);
         }   
        },
    }
  
</script>

<style scoped>
    .button {
        width: 5vw;
        height: 4vh;
    }
    p{
        margin:150px;
    }

</style>

