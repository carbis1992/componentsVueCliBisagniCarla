<template>
  <NavBar :titulo="'Home page - por ahora te quedas aca jaja'"/>
  <ListadoProductosVue />
  <!-- <MiComponente lastName="PEREZ"/>
  <EjemploWatch /> -->

  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import MiComponente from './components/MiComponente.vue';
// import EjemploWatch from "./components/EjemploWatch.vue";
import NavBar from './components/NavBar.vue';
import ListadoProductosVue from './components/ListadoProductos.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // MiComponente,
    // EjemploWatch,
    NavBar,
    ListadoProductosVue
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
</style>
