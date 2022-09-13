<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias para back-end</p>
    <ul>
        <li v-for="tecnologia in tecnologias_backend">{{tecnologia}}</li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end</p>
    <ul>
        <li v-for="tecnologia in tecnologias_frontend">{{tecnologia.linguagem}}</li>
    </ul>
    <div>
        <button @click="showEmail">{{textoBotao}}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{email}} </p>
    <p class="teste">Para acessar meu portfólio <a v-bind:href="meu_link" target="_blank">clique aqui</a></p>
    <Picture />
</template>

<script>
import Picture from './Picture.vue';
export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "ariane@email.com",
            meu_link: "https://www.google.com/",
            textoBotao: "Mostrar e-mail",
            tecnologias_backend: ["Javascript", "PHP", "Python"],
            tecnologias_frontend: [{ id: 1, linguagem: "HTML" }, { id: 2, linguagem: "CSS" }, { id: 3, linguagem: "Vue" }]
        };
    },
    components: { Picture },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if (!this.mostrar_email) {
                this.textoBotao = "Mostrar e-mail"
            } else {
                this.textoBotao = "Esconder e-mail"
            }
        }
    }
}
</script>