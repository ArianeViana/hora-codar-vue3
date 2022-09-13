<template>
    <ul>
        <li><a h-ref="">Home</a></li>
        <li><a h-ref="">Projetos</a></li>
        <li><a h-ref="">Contato</a></li>
        <li v-if="esta_logado"><a h-ref="">Meu Perfil</a></li>

    </ul>
</template>

<script>
export default {
    name: 'Header',
    props: ["esta_logado"]
}
</script>

<style scoped>
ul {
    list-style: none;
    display: flex;
    background-color: #999;
}

li {
    margin-right: 10px;
}

a {
    color: #ddd;
    text-decoration: none;
    transition: 5s;
}

a:hover {
    color: turquoise
}
</style>