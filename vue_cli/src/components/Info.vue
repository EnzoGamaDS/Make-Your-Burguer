<template>
   <div>
        <p v-if="esta_trabalhando">
            Estou trabalhando no momento
        </p>
        <p v-else>
            Não estou trabalhando
        </p>
        <p>utilizo as seguintes tecs para back end </p>
        <ul>
            <li v-for="(tec, index) in backend_tecs" v-bind:key="index">{{tec}}</li>
        </ul>
        <p>utilizo as seguintes tecs para front end </p>
        <ul>
            <li v-for="tec in frontend_tecs" :key="tec.id">
                {{tec.language}}
            </li>
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
            textoBotao: "Mostrar email",
            backend_tecs: ['PHP', 'JS', 'Java'],
            frontend_tecs: [
                {id: 1,language:'HTML'},
                {id: 2,language:'CSS'},
                {id: 3,language:'JavaScript'},
            ]
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
