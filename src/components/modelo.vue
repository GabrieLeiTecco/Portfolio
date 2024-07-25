<script setup>
import {ref} from 'vue'

const texto = ref('')
const num = ref(0)
</script>

<template>
    <input type="text" v-model="texto">
    <h1 style="font-size: larger; -webkit-text-stroke: 1px black; color: blueviolet;">{{ texto }}</h1>
    <button @click="num=Math.random()*100"> aleatório</button>
    <p>{{ num }}</p>
</template>