<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <SegundoComponente />
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import SegundoComponente from './components/SegundoComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Header from './components/Header.vue';
export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    SegundoComponente,
    LifeCycle,
    Pessoa,
    Header
  }
}
</script>

<style>
body {
  background-color: #333;
  color: #fff
}

a {
  color: red
}

.teste {
  background-color: blue;
}
</style>