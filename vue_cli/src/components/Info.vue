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
    </div>
</template>

<script>
    export default {
        name : 'Info',
        data() {
            return {
                esta_trabalhando: true,
                mostrar_email: true,
                email: 'gamaenzosw@hotmail.com'
            }
        },
    }

</script>
