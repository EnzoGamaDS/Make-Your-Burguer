<template>
    <div id="main-banner">
        <h1>Make your burguer</h1>
    </div>
</template>
<script>
    export default {
        name: "Banner"
    }
</script>

<style scoped> 
    #main-banner {
        background-image: url("/public/img/burguer.jpg");
        background-position: 0 -250px;
        background-size:cover;
        height:500px;
        display:flex;
        align-items:center;
        align-content: flex-start;
        margin: -50px -50px;
    }
    #main-banner h1 {
        color:  #FFF;
        text-align: center;
        font-size: 60px;
        background-color: #222;
        padding: 20px 40px;

    }
</style>