<template>
  <p class="card">Hola {{ prefijo }} {{ firstName }}</p>
  <p>{{ lastName }}</p>
  <button @click="añadirNuevoAlumno">Añadir a {{ newAlumno }}</button>
  <ul>
    <li v-for="(alumno, i) in alumnos" :key="i">
      <un-alumno :name="alumno" />
    </li>
  </ul>
</template>
  
<script>
  import UnAlumno from "./UnAlumno.vue";

  export default {
    name: 'MiComponente',
    components: {
      UnAlumno
    },
    props: {
      firstName: {
        type: String,
        default: "Santiago"
      },
      newAlumno: {
        type: String,
        default: "Camila"
      },
      lastName: String
    },
    data() {
      return {
        prefijo: "Mr.",
        alumnos: ['Carla', 'Leonela', 'Melisa', 'Julia']
      }
    },
    methods:{
      añadirNuevoAlumno() {
        this.alumnos.push(this.newAlumno)
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  </style>
  