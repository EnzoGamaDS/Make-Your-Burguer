<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro()"> Ativar multiplos eventos</button>
        <p>{{multiplosEventos}}</p>
    </div>    
</template>

<script>
    export default{
        name: 'Multiplos eventos',
        data() {
            return {
                multiplosEventos: "",
                txt1: "primeiro evento",
                txt2: "segundo evento"
            }
        },
        methods:{
            primeiro(txt , e){
                this.multiplosEventos = txt ;
            },
             segundo(txt , e){
                setTimeout(() => this.multiplosEventos = txt, 500);
            },
             terceiro(){
                setTimeout(() => this.multiplosEventos = "", 1500);
            }
        }
    }
    
</script>

<style scoped>
    div{
        margin: 100px;
    }

</style>>
