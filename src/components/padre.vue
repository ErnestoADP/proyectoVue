<template>
    <div>
        <button @click="mostrar = true">Mostrar componente hijo</button>
        <hijo @cerrar="mostrar = false" v-show="mostrar"></hijo>



    </div>
</template>

<script>
import hijo from "./hijo";

    export default {
        name:"padre",
        components:{
            hijo,
        },
        data(){
            return{
                mostrar: false,
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>