<script setup>
import { ref } from 'vue'

const media = ref(0)
</script>

<template>
    <h1>{{ media }}</h1>
    <button @click="media++" v-if="media < 10">Mais</button><button @click="media--" v-if="media > 0">Menos</button>
    <br>
    <h1 class="passou" v-if="media >= 6">Passou!</h1> 
    <h1 class="exame" v-else-if="media <= 5 && media >= 4">Exame.</h1>
    <h1 class="reprovado" v-else="">Não passou</h1>
    <br>
    <h2 v-if="media==0">Limite minimo de nota atingido</h2> 
    <h2 v-else-if="media==10">Limite máximo de nota atingido</h2>
    <br><br>
</template>

<style>
    h1.passou{
        color: limegreen;
        -webkit-text-stroke: 1px black;
        font-weight: bolder;
        font-family: Arial, Helvetica, sans-serif;
    } h1.exame{
        color: yellow;
        -webkit-text-stroke: 1px black;
        font-weight: bolder;
        font-family: Arial, Helvetica, sans-serif;
    } h1.reprovado{
        color: red;
        -webkit-text-stroke: 1px black;
        font-weight: bolder;
        font-family: Arial, Helvetica, sans-serif;
    }
    h2{
        color: black;
        font-weight: bolder;
        font-family: Arial, Helvetica, sans-serif;
    }
</style>