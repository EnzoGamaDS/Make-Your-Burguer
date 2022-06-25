<template>
  <div class="main-container">
  <Banner/>
    <h1>Monte seu burguer:</h1>
    <p>Formulário</p>
  </div>
</template>

<script>
  import Banner from '../components/Banner.vue'

  export default {
    name: "HomeView",
    components:{
      Banner
    }
  }
</script>
<style>
  .main-container h1 {
    margin-top: 45px;
  }

</style>