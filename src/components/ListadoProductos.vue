<template>
    <un-producto v-for="(platos, idx) of coderMeals"
        :titulo="platos.titulo"
        :portada="platos.portada"
        :costo="platos.costo"
        class="coder-meals"
        :key="idx" />
</template>

<script>
import UnProducto from './UnProducto.vue';

    export default {
        name: "ListadoProductos",
        components: {
            UnProducto
        },
        data() {
            return {
            coderMeals: [
                {
                    id: 1,
                    titulo: "Pizza napolitana",
                    costo: 930.00,
                    portada: "https://cdn0.recetasgratis.net/es/posts/5/2/6/pizza_napolitana_32625_orig.jpg"
                },
                {
                    id: 2,
                    titulo: "Spaghetti carbonara",
                    costo: 730.00,
                    portada: "https://static01.nyt.com/images/2021/02/14/dining/carbonara-horizontal/carbonara-horizontal-threeByTwoMediumAt2X-v2.jpg"
                },
                {
                    id: 3,
                    titulo: "Lasagna",
                    costo: 1200.00,
                    portada: "https://www.thewholesomedish.com/wp-content/uploads/2018/07/Best-Lasagna-550-500x375.jpg"
                },
                {
                    id: 4,
                    titulo: "Ravioles",
                    costo: 980.00,
                    portada: "https://e.rpp-noticias.io/xlarge/2020/07/15/214821_970645.jpg"
                }
            ]
        }
        }
    }
</script>

<style scoped>

</style>