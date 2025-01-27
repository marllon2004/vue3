<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{nome }} e trabalho como {{ programador }}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: "Marllon",
                profissao: "Programador"
            }
        }
    }
</script>
