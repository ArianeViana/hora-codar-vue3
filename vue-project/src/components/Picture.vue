<template>
    <!-- v-bind pode ser substituido pelo : -->
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Ariane Viana"
        }
    }
}
</script>