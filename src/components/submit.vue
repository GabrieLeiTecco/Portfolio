<script setup>

function oi(event){
  alert('oi')
  
}
</script>

<template>
  <form @submit="oi()">
    <input type="submit" value="Enviar">
  </form>
</template>
