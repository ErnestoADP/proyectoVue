<template>
    <div>
            <h2>Soy el componente hijo</h2>
            <button @click="emitirEvento"> cerrar hijo</button>
    </div>
</template>

<script>
    export default {
        name:"hijo",
        methods:{
            emitirEvento(){
                this.$emit('cerrar')
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>