<template>
    <Navbar :logo="img_logo" :alt="app_name" />
    <router-view />
    <Footer />

</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
    components: {
        Navbar,
        Footer
    },
    data() {
        return {
            app_name: "Make Your Burguer",
            img_logo: "/img/logo.png"
        }
    }
}
</script>

<style>
* {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

.main-container {
    margin: 50px;
    min-height: 250px;
}

h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
    margin-top: 25px;
}
</style>