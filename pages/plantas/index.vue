<template>
    <div>
        <h2>¿Plantas?</h2>
      <div>
    <v-list>
        <v-list-item
        v-for="planta in plantas" :key="planta.nombre"
        :to="{path: '/plantas/' + planta.nombre,
        query: {}}">
        <v-list-item-content>
            <v-list-item-title>{{planta.nombre}}</v-list-item-title>
        </v-list-item-content>
       </v-list-item>
    </v-list>
    </div>
   </div> 
</template>

<script>


export default{
    data(){
        return{
            plantas:[
                {nombre: 'Clematis',
                familia: 'Clematidae',
                },
                {nombre: 'Malva paciflora',
                 familia: 'malvaceae'
                }
            ]
        }
    }
}
</script>
