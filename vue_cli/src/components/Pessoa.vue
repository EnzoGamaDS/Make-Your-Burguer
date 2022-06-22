<template>
    <div>
        <h2>
            Essa é a descrição da Pessoa : {{nome}}
        </h2>
        <Info :email="email" :esta_trabalhando="true"/>
    </div>
</template>

<script>
import Info from './Info.vue';
    export default {
    name: "Pessoa",
    components: {
        Info
    },
    data() {
        return {
            nome: "Enzinho delax",
            email:"gamagamgama@gama.com"
        };
    },
    components: { Info }
}

</script>