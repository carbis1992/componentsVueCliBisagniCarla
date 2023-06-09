<template>
    <h1 class="titulo">{{titulo}}</h1>
    <div class="navbar">
        <a class="item-navbar">Index</a>
        <a class="item-navbar">Contact</a>
        <a class="item-navbar">anchor</a>
    </div>
</template>

<script>
    export default {
        name: "NavBar",
        props: {
            titulo: String
        }
    }
</script>

<style scoped>
    .titulo{
    text-align: center;
    }

    .navbar{
    display: flex;
    justify-content: space-between;
    border-bottom: 1px solid lightgray;
    padding: 12px;
    }

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
</style>