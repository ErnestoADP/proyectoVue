

<script>
    export default {
        name :'elementorender',
        props:['tipo'],
        render(createElement){
            return createElement(
                this.tipo,   //el tipo de elemento que va a renderizar
                this.$slots.default,  //contenido del elemento a renderizar
            )
        }
    }
</script>

<style  scoped> /*scoped previene que los elementos css se propaguen por todos los componentes*/ 

h1,h2{
    color:rebeccapurple;
}

p{
    color: blue;
}

</style>