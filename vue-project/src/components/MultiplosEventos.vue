<template>
    <div>
        <button @click="primeiro(), segundo(txt)">Ativar múltiplos eventos</button>
        <p>{{multiplos_eventos}}</p>

    </div>
</template>

<script>
export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: "",
            txt: "segundo evento"
        }
    },
    methods: {
        primeiro() {
            this.multiplos_eventos = "Primeiro evento ativado"
        },
        segundo(txt) {
            setTimeout(() => { this.multiplos_eventos = txt }, 700)
        }
    }
}
</script>

<style scoped>
div {
    margin: 100px
}
</style>