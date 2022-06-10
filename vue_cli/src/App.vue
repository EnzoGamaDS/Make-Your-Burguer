<template>
  <div>
    <PrimeiroComponente/>
    <HelloWorldVue/>
    <PessoaVue/>
  </div>
</template>

<script>
import PrimeiroComponente  from './components/PrimeiroComponente.vue'
import HelloWorldVue from './components/HelloWorld.vue'
import PessoaVue from './components/Pessoa.vue'
export default {
  name : 'App',
  components : {
    PrimeiroComponente,
    HelloWorldVue,
    PessoaVue
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
