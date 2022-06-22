<template>
    <div>
        <button @click="Ativar">CLicke aqui !</button>
        <span v-show="ativou">Ativado</span>
    </div>
</template>

<script>
    export default {
    name:'Reutilizacao',
    data() {
        return {
            ativou: false      
        }
    },
    methods: {
        Ativar() {
            this.ativou = !this.ativou;
        }
        }
    }

</script>