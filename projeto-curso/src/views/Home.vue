<template>
  <div class="main-container">
    <Banner />
    <h1>Monte o seu Burger:</h1>
    <Form />
  </div>
</template>

<script>
import Banner from '../components/Banner.vue';
import Form from '../components/Form.vue';

export default {
  name: 'Home',
  components: {
    Banner,
    Form
  }
}

</script>

