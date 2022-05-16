      <div>
         <vehiculo
            v-for="(item, i) in Vehiculo"
            :key="i"
            :id="item.id"
            :marca="item.marca"
            :precio="item.precio"
            :modelo="item.modelo"
         >
         </vehiculo>
      </div>






        Vehiculo: {

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
                },






clase vehiculo

            <table :class="estilos">
                <thead >
                    <tr>
                        <th v-for="(item, i) in titulos" :key="i" scope="col">{{ item }}</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="(unidad, u) in vehiculo" :key="u">
                        <th>{{ u + 1 }}</th>
                        <th>{{ unidad.marca }}</th>
                        <th>{{ unidad.modelo }}</th>
                        <th>{{ unidad.precio }}</th>
                    </tr>
                </tbody>
            </table>



app vue
         <vehiculo
            v-for="(item, i) in Vehiculo"
            :key="i"
            :id="item.id"
            :marca="item.marca"
            :precio="item.precio"
            :modelo="item.modelo"
         >
         </vehiculo>

            <table :class="estilos">
                <thead >
                    <tr>
                        <th v-for="(item, i) in titulos" :key="i" scope="col">{{ item }}</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="(unidad, u) in vehiculo" :key="u">
                        <th>{{ u + 1 }}</th>
                        <th>{{ unidad.marca }}</th>
                        <th>{{ unidad.modelo }}</th>
                        <th>{{ unidad.precio }}</th>
                    </tr>
                </tbody>
            </table>
<h1>{{ titulos }}</h1>
<h1>{{ vehiculo }}</h1>

            <tabla-vehiculo :titulos="tabla1.titulos" :registros="tabla1.vehiculo" :estilos="'table-info blue'">
            </tabla-vehiculo>

            <tabla-vehiculo :titulos="tabla2.titulos" :registros="tabla2.vehiculo" :estilos="'table-info green'">
            </tabla-vehiculo>

            <tabla-vehiculo :titulos="tabla3.titulos" :registros="tabla3.vehiculo" :estilos="'table-info orange'">
            </tabla-vehiculo>

