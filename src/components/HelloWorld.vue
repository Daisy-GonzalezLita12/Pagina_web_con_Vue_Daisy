<script setup>
import card from '../components/card.vue'
import cardPrincipal from '../components/CardPrincipal.vue'
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
    <!--Mandamos a llamar el componente cardPrincipal -->
       <card-principal/>
   <!--Mandamos a llamar el componente card -->
   <!-- card1 -->
    <card/>


  </div>
</template>
<style scoped>
</style>
