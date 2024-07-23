<script setup>
    import { ref } from 'vue'
    const a = ref(0)
    const b = ref(1)
</script>

<template>
    <button @click="a++">Mais</button>
    <button @click="a--">Menos</button>
    <button @click="b=b*-1">Olho</button>
    <br>
    <button @click="a=a/2">Divide</button>
    <button @click="a=a*a">Exponencia</button>
    <button @click="a=0">Zera</button>
    <br><br>

    <h1 v-if="b==1">{{ a }}</h1>
</template>