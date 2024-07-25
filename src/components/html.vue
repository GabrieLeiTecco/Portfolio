<script setup>
let html = '<p style="color: red;">Batata</p><h1>1 2 3 4</h1>'
</script>

<template>
    <div v-html="html"></div>
    <div>{{ html }}</div>
</template>