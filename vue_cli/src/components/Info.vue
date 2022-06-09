<template>
   <div>
        <p v-if="esta_trabalhando">
            Estou trabalhando no momento
        </p>
        <p v-else>
            Não estou trabalhando
        </p>
        <ul>
            <li>JS</li>
            <li>PHP</li>
            <li>Pitao</li>
        </ul>
        <div>
            <button @click="showEmail">{{textoBotao}}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
        <p>Para acessar meu portifólio <a v-bind:href="meu_link">basta clickar aqui</a></p>
        <Picture/>
    </div>
</template>

<script>
import Picture from './Picture.vue'
    export default {
    components: { 
        Picture 
        },
    name: "Info",
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: "gamaenzosw@hotmail.com",
            meu_link: "https://google.com",
            textoBotao: "Mostrar email"
        };
    },
    methods: {
        showEmail(){
            this.mostrar_email = !this.mostrar_email;
            if(!mostrar_email){
                this.textoBotao = 'Mostrar email';
            }else{
                this.textoBotao = 'Esconder email';
            }
        }
    }
}

</script>
