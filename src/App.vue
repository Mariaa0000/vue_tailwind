<template>
  <div id="app">
    <vue-good-table
      :columns="columns"
      :rows="rows"
    />
  </div>
</template>

<script>
import { VueGoodTable } from 'vue-good-table-next'
import 'vue-good-table-next/dist/vue-good-table-next.css'

export default {
  name: 'Alumnos',
  components: {
    VueGoodTable,
  },
  data() {
    return {
      columns: [
        { label: 'Nombre', field: 'nombre' },
        { label: 'Teléfono', field: 'telefono' },
        { label: 'Edad', field: 'edad', type: 'number' },
        { label: 'Email', field: 'email' },
        { label: 'Género', field: 'genero' },
      ],
      rows: [
  { id:1, telefono:"5552193642", nombre:"Alumno1", edad: 78, email:"alumno1@ejemplo.com", genero:"F" },
  { id:2, telefono:"5558815660", nombre:"Alumno2", edad: 57, email:"alumno2@ejemplo.com", genero:"M" },
  { id:3, telefono:"5553052938", nombre:"Alumno3", edad: 24, email:"alumno3@ejemplo.com", genero:"F" },
  { id:4, telefono:"5553155871", nombre:"Alumno4", edad: 68, email:"alumno4@ejemplo.com", genero:"F" },
  { id:5, telefono:"5551056625", nombre:"Alumno5", edad: 66, email:"alumno5@ejemplo.com", genero:"M" },
  { id:6, telefono:"5551658141", nombre:"Alumno6", edad: 66, email:"alumno6@ejemplo.com", genero:"F" },
  { id:7, telefono:"5557633161", nombre:"Alumno7", edad: 33, email:"alumno7@ejemplo.com", genero:"F" },
  { id:8, telefono:"5556778150", nombre:"Alumno8", edad: 65, email:"alumno8@ejemplo.com", genero:"F" },
  { id:9, telefono:"5559367319", nombre:"Alumno9", edad: 31, email:"alumno9@ejemplo.com", genero:"F" },
  { id:10, telefono:"5553175476", nombre:"Alumno10", edad: 40, email:"alumno10@ejemplo.com", genero:"F" },
]

    }
  }
}
</script>
