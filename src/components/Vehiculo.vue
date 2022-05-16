<template>
<div>

</div>

</template>

<script>
export default {
  name: 'Vehiculo',
    props:{
        titulos: {
            type: Array,
            required: true
        },
        vehiculo:{
            type: Array,
            required: true
        },
        estilos:{
            type: String,
            required: true
        }

    },
};
data:{
      tabla1: {
            titulos: ["Opcion", "Marca", "Modelo", "Precio"],
            vehiculo [
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

      };
        tabla2: {
            titulos: ['Opcion', 'Motor', 'Caja', 'Combustible'],
            vehiculo [
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
        };
        tabla3: {
            titulos: ['Opcion', 'GPS', 'ABS', 'ESP'],
            vehiculo [
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
        };

</script>


<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
