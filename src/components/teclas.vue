<script setup>
    function validar() {
        var a = document.getElementById('txt').value
        const padraoSenha = /\W|_/
        if (padraoSenha.test(a) == true) {
            alert('Senha forte!')
        }else{
            alert('Senha fraca!')
        }
    }
</script>

<template>
    <input id="txt" type="text" @keyup.enter="validar()" placeholder="DIgite sua senha depois pressione 'enter'">
</template>