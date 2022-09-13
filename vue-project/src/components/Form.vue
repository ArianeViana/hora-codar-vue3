<template>
    <form action="" @submit="enviarForm($event)">
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <input type="text" v-model="email">
        </div>
        <div>
            <Submit />
        </div>
    </form>
</template>

<script>
import InputText from './form/InputText.vue';
import Submit from './form/Submit.vue';

export default {
    name: 'Form',
    data() {
        return {
            name: "",
            email: ""
        }
    },
    components: {
        InputText,
        Submit
    },
    methods: {
        enviarForm(e) {
            e.preventDefault();

            const name = this.name;
            const email = this.email;

            console.log("Formaulário enviado!");
            console.log(name)
            console.log(email)
        }
    }

}
</script>