<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar: "/images/avatar.png",
            descricao: "Enzo Gama"
        }
    },
}
</script>