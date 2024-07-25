<script setup>
import {ref} from 'vue'

let validacao = ref(1)
</script>

<style>
.foi{
    color: green;
} .nfoi{
    color: red;
}
</style>

<template>
    <h1 v-bind:class="validacao==1 ? 'foi' : 'nfoi'">Foi</h1>
    <h1 class="mexe" v-bind:draggable="validacao==1 ? true : false">Mexe</h1>
    <button @click="validacao=validacao*-1">Clica</button>
</template>