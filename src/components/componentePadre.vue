<template>
    <div>   
        <p>el nombre es: {{nombre}}</p>
        <p>la edad es: {{edad}}</p>
        <componenteHijo :nombre="nombre" :edad="edad" ></componenteHijo>

    </div>
</template>

<script>

import componenteHijo from "./componenteHijo";

    export default {
        name:"componentePadre",
        props:['nombre','edad'],    
        components:{componenteHijo}
    }
</script>

<style lang="scss" scoped>

</style>