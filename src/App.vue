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
