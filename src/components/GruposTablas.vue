<template>
    <table class="grupo-tabla">
                <thead :class="thead(index)">
                <tr>
                    <th v-for="(title, i) in titulos" :key="i">{{ title }}</th>
                </tr>
                </thead>
        
                <tbody>
                <tr :class="resaltarArgentina(registro.localidad1, registro.localidad2)" v-for="(registro, i) in registros" :key="registro.id">
                    <td>{{ i + 1}}</td>
                    <td>{{ registro.localidad1}}</td>
                    <td>{{ registro.localidad2 }}</td>
                    <td>{{ registro.resultado }}</td>
                </tr>
                </tbody>
            </table>  
</template>

<script>
export default {
    props:{
        titulos:{
            type: Array,
            required: true
        },
        registros:{
            type: Array,
            required: true
        },
        index:{
            type: Number
        }
    },
    methods: {
        thead(index) {
            return index % 2 == 0 ? 'thead-dark' : 'thead-light' 
          
        },
        resaltarArgentina(pais1, pais2) {
            if (pais1 == "Argentina" || pais2 == "Argentina")
                return 'argentina'
        }
      }, 


}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Koulen&display=swap');

.contenedor-grupos{
    display: flex;
    justify-content: center;
}
.grupo-tabla{
    margin: 1rem;
    font-family: 'Koulen', cursive;
    font-size: 20px;
}
.grupo{
    display: flex;
    justify-content: center;
    font-family: 'Koulen', cursive;
}
th{
    width: 15rem;
}
.thead-dark{
    background: pink;
}
.thead-light{
    background: magenta;
}
.fila-par{
    background: white;
}
.fila-impar{
    background: grey;
}
.argentina{
    background: grey;
    color: blue;
}


</style>