<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{nome}}</h2>
        <Info emailSecundario="arianeSecundario@email" />
        <Form />
    </div>
</template>

<script>
import Info from './Info.vue';
import Form from './Form.vue';
export default {
    name: "Pessoa",
    data() {
        return {
            nome: "Ariane"
        };
    },
    components: { Info, Form }
}
</script>