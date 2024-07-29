<script setup>
function clicou() {
    alert('Clicou!')
}
</script>

<template>
    <!--'@' serve para usarmos eventos como "Click"-->
    <button @click="clicou()">Clica</button>
</template>