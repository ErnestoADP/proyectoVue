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
        props:['id','nombre','email','telefono']
    }
</script>

<style lang="scss" scoped>

</style>