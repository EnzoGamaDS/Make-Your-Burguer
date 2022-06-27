<template>
  <div class="main-container">
    <Banner/>
    <h1>Monte seu burguer:</h1>
    <p>Formulário</p>
    <BurguerForm/>
  </div>
</template>

<script>
  import Banner from '../components/Banner.vue'
  import BurguerForm from '../components/BurguerForm.vue'

  export default {
    name: "HomeView",
    components:{
      Banner, BurguerForm
    }
  }
</script>
<style>
  .main-container h1 {
    margin-top: 45px;
  }

</style>