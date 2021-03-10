<template>
  <div>
    <saludos></saludos>
    <saludoDos></saludoDos>
    <hr>
    <h1>Componentes</h1>

   <componentePadre nombre="Manuel" edad="45"></componentePadre>
   <hr>
   <componentePadre nombre="jose" edad="56"></componentePadre>
   <hr>
   <componentePadre nombre="rodrigo" edad="34"></componentePadre>
   <hr>
  </div>


</template>

<script>
import saludos from "./components/saludos"; 
import saludoDos from "./components/saludoDos";
import ComponentePadre from './components/componentePadre';





export default {
  name: 'App',
  components: {
    saludos,
    saludoDos,
    ComponentePadre,
 
    
 
   
  }
}
</script>

<style>

</style>
