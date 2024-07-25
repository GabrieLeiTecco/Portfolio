<script setup>
    let nomes = ['Gabriel', 'Amanda', 'Lucas', 'João', 'Otaku']
</script>

<template>
    <ul>
        <li v-for="amigo in nomes">{{ amigo }}</li>
    </ul>
</template>