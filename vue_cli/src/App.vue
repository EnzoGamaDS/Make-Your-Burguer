<template>
  <div>
    <PrimeiroComponente/>
    <HelloWorldVue/>
  </div>
</template>

<script>
import PrimeiroComponente  from './components/PrimeiroComponente.vue'
import HelloWorldVue from './components/HelloWorld.vue'
export default {
  name : 'App',
  components : {
    PrimeiroComponente,
    HelloWorldVue
  }
}
</script>
