<template>
    <input v-model="value">
    <p>{{ value }}</p>
</template>

<script>
    export default {
        name: "EjemploWatch",
        data() {
            return {
                value: ''
            }
        },
        watch: {
            value(newVal) {
                console.log("ey", newVal);
            }
        }
    }
</script>