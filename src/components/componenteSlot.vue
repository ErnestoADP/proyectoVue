<template>
    <div>
        <h1 style="color:red">
            <slot>
                hola desde el componente
            </slot>

        </h1>

       

        <h2>
            <slot name="slotdo2">
                hola desde el componente 2
            </slot>

        </h2>

    </div>
</template>

<script>
    export default {
        name:"componenteSlot"
    }
</script>

<style lang="scss" scoped>

</style>