<template>
    <div>
        <table :class="estilos">
            <thead >
                <tr>
                    <th v-for="(item, i) in titulos" :key="i" scope="col">{{ item }}</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(unidad, u) in vehiculos" :key="u">
                    <th>{{ u + 1 }}</th>
                    <th>{{ unidad.marca }}</th>
                    <th>{{ unidad.modelo }}</th>
                    <th>{{ unidad.precio }}</th>
                </tr>
            </tbody>
        </table>
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
        vehiculos:{
            type: Array,
            required: true
        },
        estilos:{
            type: String,
            required: true
        }

    },
};

</script>

<style scoped>
    .table-info{
        width: 100%;
        border: 1px solid #999;
        text-align: left;
        border-collapse: collapse;
        margin: 0 0 1em 0;
        border-color: black;
    }

    .table-info.green th{
        background-color: rgb(221, 240, 221);
    }
    .table-info.blue th{
        background-color: rgb(165, 187, 235);
    }
    .table-info.orange th{
        background-color: rgb(238, 164, 133);

    }

    .table-info th{
        text-align: center;
        border: solid rgb(90, 90, 90) 1px;
    }
</style>
