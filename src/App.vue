<template>
  <div id="app">
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <TitleHeading titulo="Prode - Mundial Qatar 2022"/>
    <GruposTablas />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TitleHeading from './components/TitleHeading.vue'
import GruposTablas from './components/GruposTablas.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    TitleHeading,
    GruposTablas
  },
  data() {
          return {
              titulos: ["ID","Pais 1","Pais 2","Resultado"],
              tablas: [
                  {
                      registros:[
                          {
                              id: 1,
                              localidad1: "Qatar",
                              localidad2: "Ecuador",
                              resultado: "1-0"
                          },
                          {
                              id: 2,
                              localidad1: "Senegal",
                              localidad2: "Paises Bajos",
                              resultado: "1-2"
                          },
                          {
                              id: 3,
                              localidad1: "Qatar",
                              localidad2: "Senegal",
                              resultado: "1-0"
                          },
                          {
                              id: 4,
                              localidad1: "Ecuador",
                              localidad2: "Paises Bajos",
                              resultado: "0-3"
                          },
                          {
                              id: 5,
                              localidad1: "Qatar",
                              localidad2: "Paises Bajos",
                              resultado: "1-2"
                          },
                          {
                              id: 6,
                              localidad1: "Ecuador",
                              localidad2: "Senegal",
                              resultado: "0-1"
                          }
                      ]
                  },
                  {
                      registros:[
                          {
                              id: 7,
                              localidad1: "Inglaterra",
                              localidad2: "Iran",
                              resultado: "1-1"
                          },
                          {
                              id: 8,
                              localidad1: "Estados Unidos",
                              localidad2: "Repesca",
                              resultado: "1-0"
                          },
                          {
                              id: 9,
                              localidad1: "Inglaterra",
                              localidad2: "Estados Unidos",
                              resultado: "2-0"
                          },
                          {
                              id: 10,
                              localidad1: "Iran",
                              localidad2: "Repesca",
                              resultado: "1-1"
                          },
                          {
                              id: 11,
                              localidad1: "Inglaterra",
                              localidad2: "Repesca",
                              resultado: "1-0"
                          },
                          {
                              id: 12,
                              localidad1: "Iran",
                              localidad2: "Estados Unidos",
                              resultado: "1-0"
                          }
                      ]
                  },
                  {
                      registros:[
                          {
                              id: 13,
                              localidad1: "Argentina",
                              localidad2: "Arabia Saudi",
                              resultado: "3-0"
                          },
                          {
                              id: 14,
                              localidad1: "Mexico",
                              localidad2: "Polonia",
                              resultado: "1-0"
                          },
                          {
                              id: 15,
                              localidad1: "Argentina",
                              localidad2: "Mexico",
                              resultado: "2-0"
                          },
                          {
                              id: 16,
                              localidad1: "Arabia Saudi",
                              localidad2: "Polonia",
                              resultado: "1-2"
                          },
                          {
                              id: 17,
                              localidad1: "Argentina",
                              localidad2: "Polonia",
                              resultado: "2-0"
                          },
                          {
                              id: 18,
                              localidad1: "Arabia Saudi",
                              localidad2: "Mexico",
                              resultado: "1-0"
                          }
                      ]
                  }
              ]
          }
      },
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
