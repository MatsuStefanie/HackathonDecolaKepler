<template>
  <img alt="Vue logo" src="./assets/octacatmatsu.png" class="logo">
  <HelloWorld msg="Seja bem vindo, welcome a new project in vue"/>
  <NovoComponente />
  <TesteIf />
  <TesteFor />
  <TesteEvents />
  <TesteConsumoAPI />
  <UmContador />
</template>

<script>
  import HelloWorld from './components/HelloWorld'
  import NovoComponente from './components/NovoComponente'
  import TesteIf from './components/TesteIf.vue'
  import TesteFor from './components/TesteFor'
  import TesteEvents from './components/TesteEvents'
  import TesteConsumoAPI from './components/TesteConsumoAPI'
  import UmContador from './components/UmContador'


  export default {
    name: 'App',
    components: {
      HelloWorld,
      NovoComponente,
      TesteIf,
      TesteFor,
      TesteEvents,
      TesteConsumoAPI,
      UmContador
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  .logo{
    width: 100px;
    height: 100px;
  }
</style>
