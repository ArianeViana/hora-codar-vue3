<template>
    <div>
        <Reutilizacao />
        <h1>Olá, Vue!</h1>
        <p>Meu nome é {{nome}}</p>
        <p>E trabalho com {{profissao}}</p>
        <MultiplosEventos />
        <Reutilizacao />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reutilizacao from './Reutilizacao.vue';
export default {
    name: "PrimeiroComponente",
    data() {
        return {
            nome: "Ariane",
            profissao: "Programação"
        };
    },
    components: { MultiplosEventos, Reutilizacao }
}
</script>