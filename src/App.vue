<template>
  <div id="app">
    <Vehiculo :titulos="tabla1.titulos" :vehiculos="tabla1.vehiculo" :estilos="'table-info blue'">
    </Vehiculo>

    <Vehiculo :titulos="tabla2.titulos" :vehiculos="tabla2.vehiculo" :estilos="'table-info green'">
    </Vehiculo>

    <Vehiculo :titulos="tabla3.titulos" :vehiculos="tabla3.vehiculo" :estilos="'table-info orange'">
    </Vehiculo>
  </div>
</template>

<script>
import Vehiculo from './components/Vehiculo.vue';

export default {
name: 'App',
  components: {
    Vehiculo,
  },

    data: () => ({
            tabla1: {
                titulos: ["Opcion", "Marca", "Modelo", "Precio"],
                vehiculo: [
                    {
                        marca: 'Fiat',
                        modelo: ' Uno Way',
                        precio: 850000
                    },
                    {
                        marca: 'Ford',
                        modelo: 'Fiesta Kinetic',
                        precio: 1750000
                    },
                    {
                        marca: 'Volskwagen',
                        modelo: 'Nivus',
                        precio: 2600000
                    }

                ]

            },
            tabla2: {
                titulos: ['Opcion', 'Motor', 'Caja', 'Combustible'],
                vehiculo: [
                    {
                        marca: 'Motor 1.4',
                        modelo: '5 velocidades Manual',
                        precio: 45 //combustible
                    },
                    {
                        marca: 'Motor 1.6',
                        modelo: '6 velocidades Automatica',
                        precio: 52
                    },
                    {
                        marca: 'Motor 1.0',
                        modelo: '6 Velocidades Manual',
                        precio: 55
                    }
                ]
            },
            tabla3: {
                titulos: ['Opcion', 'GPS', 'ABS', 'ESP'],
                vehiculo: [
                    {
                        marca: 'No',
                        modelo: 'Si',
                        precio: 'No'
                    },
                    {
                        marca: 'Si',
                        modelo: 'Si',
                        precio: 'No'
                    },
                    {
                        marca: 'Si',
                        modelo: 'Si',
                        precio: 'Si'
                    }
                ]
            },
        })
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
