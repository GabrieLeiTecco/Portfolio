<script setup>
import { onMounted, ref } from 'vue'

var timer = 0
onMounted(()=>{
  setTimeout(()=>{
    timer++
  }, 1000)
})
</script>

<template>
  <div>
    {{timer}}
  </div>
</template>
