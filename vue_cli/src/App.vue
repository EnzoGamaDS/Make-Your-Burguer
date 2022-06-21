<template>
  <div>
    <PrimeiroComponente/>
    <HelloWorldVue/>
    <PessoaVue/>
    <FormVue/>
  </div>
</template>

<script>
import PrimeiroComponente  from './components/PrimeiroComponente.vue'
import HelloWorldVue from './components/HelloWorld.vue'
import PessoaVue from './components/Pessoa.vue'
import FormVue from './components/Form.vue'
export default {
  name : 'App',
  components : {
    PrimeiroComponente,
    HelloWorldVue,
    PessoaVue,
    FormVue
  }
}
</script>

<style>
  body{
    background-color: #333; 
    color: #FFF;
  }
  a{
    color: red;
  }
</style>
