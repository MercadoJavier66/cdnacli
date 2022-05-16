<template>
  <div id="app">

    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Esto es Cli con Vue 2"/>
    <h3>monty pierde la cabeza</h3>

    <HelloWorld msg="hola" >

    </HelloWorld >
    <Vehiculo >
    </Vehiculo >

  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Vehiculo from './components/Vehiculo.vue';

export default {
name: 'App',
  components: {
      HelloWorld,
    Vehiculo,
  },

// data() {
//     return{
//          numeroA: 1
//     }
//   }
};


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
