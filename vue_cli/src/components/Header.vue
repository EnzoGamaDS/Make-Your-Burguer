<templete>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
    </ul>

</templete>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background: #999;
    }
    li{
        margin-right: 10px;
    }
    a{
        color: #ddd;
        transition: .5s;
    }
    a:hover{
        color: turquoise;
    }
</style>