<template>
    <div>
        <p>monte seu form</p>
        <div>
            <form id="burguer-form">
                <div class="input-container">
                    <label for="nome">Nome do cliente</label>
                    <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu nome">
                </div>
                <div class="input-container">
                    <label for="pao">Escolha o pão</label>
                    <select name="pao" id="pao">
                        <option value="">Selecione o seu pão</option>
                        <option value="integral">Integral</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="carne">Escolha a carne</label>
                    <select name="carne" id="carne">
                        <option value="">Selecione o tipo de carne</option>
                        <option value="maminha">maminha</option>
                    </select>
                </div>
                <div id="opcionais-container" class="input-container">
                    <label id="opcionais-title" for="opcionais">Escolha os opcionais</label>
                    <div class="checkbox-container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                    <div class="checkbox-container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                    <div class="checkbox-container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                </div>
                <div>
                    <input type="submit" class="submit-btn" value="Criar meu burguer">
                </div>
            </form>
        </div>
    </div>    
</template>
<script>
export default {
    name:'BuerguerForm'        
 }
</script>
<style scoped>
#burguer-form {
    max-width: 400px;
    margin: 0 auto;
}
.input-container{
    display: flex;
    flex-direction:column;
    margin-bottom: 20px;
}
.input-container input,
.input-container select{
    height: 4vh;
    padding-left: 10px;
}
label{
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    padding: 5px 10px;
    border-left: 4px solid #fcba03;
}
input select {
    padding: 5px 10px;
    width: 300px;
}
#opcionais-container{
    flex-direction: row;
    flex-wrap:wrap;
}
#opcionais-title{
    width: 100%;
}
.checkbox-container{
    display: flex;
    align-items: flex-start;
    widows: 50%;
    margin-bottom: 20px;
}
.checkbox-container span,
.checkbox-container input{
    margin-right: 10px;
    width: auto;
}

.checkbox-container span{
    margin-left:50px;
    font-weight: bold;
}
.submit-btn{
    background: #222;
    color: #fcba03;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    font-size: 16px;
    margin: 0 auto;
    cursor: pointer;
    transition: 0.5s;
}
.submit-btn:hover{
    background: transparent;
    color: #222;
}
</style>