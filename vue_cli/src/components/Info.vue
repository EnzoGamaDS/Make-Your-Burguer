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
        <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
        <p>Para acessar meu portifólio <a v-bind:href="meu_link">basta clickar aqui</a></p>
        <Picture/>
    </div>
</template>

<script>
import Picture from './Picture.vue'
    components: { 
        Picture 
        }
    export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            email: "gamaenzosw@hotmail.com",
            meu_link: "https://google.com"
        };
    },
}

</script>
