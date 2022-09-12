<template>
    <div>
        <h1>Olá, Vue!</h1>
        <p>Meu nome é {{nome}}</p>
        <p>E trabalho com {{profissao}}</p>
    </div>
</template>

<script>
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            nome: "Ariane",
            profissao: "Programação"
        }
    }
}
</script>