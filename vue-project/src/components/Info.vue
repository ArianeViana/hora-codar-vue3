<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias</p>
    <ul>
        <li>Java</li>
        <li>React</li>
        <li>C#</li>
        <li>Vue.js</li>
    </ul>
    <p v-show="mandar_email">Mande uma mensagem para: {{email}} </p>
</template>

<script>
export default {
    name: 'Info',
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "ariane@email.com"
        }
    }
}
</script>