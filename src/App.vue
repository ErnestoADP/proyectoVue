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
   <hr>
   <hr>
   <hr>
   <hr>

   <h1>Traer datos desde una API</h1>

   <usuarios 
              v-for="usuario in usuarios" 
              v-bind:key="usuario.id"
                 :id="usuario.id"
                 :nombre="usuario.name"
                 :email="usuario.email"
                 :telefono="usuario.phone"    
              >  
              </usuarios>

              <hr>

 <hr>
        <hr>
        <hr>
        <hr>
        <hr>
        <hr>

        <h1>clase de componentes</h1>
        <hr>
 <componenteSlot>
   hola desde slot 

   <template slot="slotdos">


   </template>

 </componenteSlot>




  </div>

</template>

<script>
import axios from 'axios'
import saludos from "./components/saludos"; 
import saludoDos from "./components/saludoDos";
import ComponentePadre from './components/componentePadre';
import usuarios from './components/usuarios';
import ComponenteSlot from './components/componenteSlot';





export default {
  name: 'App',
  components: {
    saludos,
    saludoDos,
    ComponentePadre,
    usuarios,
    ComponenteSlot,
    
 
    
 

  },
  data(){
    return{
      usuarios:[],

    }

  },
  methods:{
    obtenerUsuarios(){
            axios.get('https://jsonplaceholder.typicode.com/users')
          .then((respuestas) => this.usuarios = respuestas.data)
    }
  },

  //se monta este componente para que ObtenerUsuario(funcion) haga una llamada a la API
  mounted(){
      this.obtenerUsuarios()
  }

}
</script>

<style>

h1
{color: red;

}

</style>
