<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Quadrado :numero = "5"/>
    <Cubo :numero = "5"/>
    <Fatorial :numero = "5"/>  
    <Primo :numero = "5"/>    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Quadrado from './components/Quadrado.vue'
import Cubo from './components/Cubo.vue'
import Fatorial from './components/Fatorial.vue'
import Primo from './components/Primo.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Quadrado,
    Cubo,
    Fatorial,
    Primo
  },
  props:{
    numero: Number
  },
  methods:{
    calcular_dobro(){
      return this.n*2
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
div{
  align-content: space-between;
  display: flex;
}
</style>
