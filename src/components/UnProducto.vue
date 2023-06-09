<template>
    <div style="text-align: center;">
        <img v-bind:src="portada" class="img-card">
        <br />
        <p>{{titulo}}</p>
        <p>$<strong>{{costo}}</strong></p>
        <button class="item-navbar">Agregar</button>
    </div>
</template>

<script>
    export default {
        name: "UnProducto",
        props: {
            portada: String,
            titulo: String,
            costo: Number
        }
    }
</script>

<style scoped>
    .item-navbar{
        text-decoration: none;
        color: black;
        padding: 10px;
        border-radius: 20%;
    }

    .item-navbar:hover{
        background-color: rgba(189, 245, 216, 0.37);
    }

    .item-navbar::after{
        text-decoration: none;
    }

    .img-card{
        width: 220px;
    }

    button{
        border: none;
        text-decoration: none;
        background: none;
    }
</style>