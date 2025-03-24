<script setup>
import card from '../components/card.vue'
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>
<template>
  <!-- Estructura html -->
   <div  class="container">
    <!-- Título de la página web -->
    <h1 style="color: #31827c;" class="text-center">MASCOTAS</h1>
    <!--Inicio del primer row  -->
   <div class="row">
       <div class="col-md-6">
        <div class="card">
          <div style="background-color: #95c68f;" class="card-header">
            <h6><center>Gatos</center></h6>
          </div>
          <div style="background-color: #f7e9aa;" class="card-body text-center">
            <!-- Imagen de un gatito -->
            <img src="https://i.pinimg.com/474x/29/41/b0/2941b0a266c0fc1cb388429315b9ccf9.jpg" alt="Gato" width="150px" height="200px"> 
            <!-- Descripción de los gatos -->
            <p class="card-text">El gato doméstico (Felis silvestris catus), llamado comúnmente gato, es un mamífero carnívoro de la familia Felidae.</p>
          </div>
        </div>
       </div>
       <div class="col-md-6">
        <div class="card">
          <div style="background-color: #95c68f;" class="card-header">
            <h6><center>Perros</center></h6>
          </div>
          <div style="background-color: #f7e9aa;" class="card-body text-center">
            <!-- Imgagen de un perrito -->
            <img src="https://i.pinimg.com/736x/96/75/74/967574cf74089714b4b13d8fb2513d8c.jpg" alt="perro" width="150px" height="200px">
          <!-- Descripción de un perrito -->
            <p class="card-text">El perro (Canis familiaris o Canis lupus familiaris). Es un mamífero carnívoro de la familia de los cánidos, que constituye una especie del género Canis.</p>
          </div>
        </div>
       </div>
   </div>
   <!-- Cierre del  primer row-->
    
   <!--Mandamos a llamar el componente card -->
   <!-- card1 -->
    <card/>

  </div>
</template>
<style scoped>
</style>
