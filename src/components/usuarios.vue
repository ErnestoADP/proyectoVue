<template>
    <div>
                <P>Id: {{id}}</P>
                <P>Nombre: {{nombre}}</P>
                <p>Email: {{email}}</p>
                <p>Telefono: {{telefono}}</p>
                <hr>
                
    </div>
</template>

<script>
    export default {
        name:"usuarios",
        props:{
                id:{type:Number},
                nombre:String,
                email:String,
                telefono:String
        }
    }
</script>

<style lang="scss" scoped>

</style>