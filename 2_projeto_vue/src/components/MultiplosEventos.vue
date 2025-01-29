<template>
    <div>
        <button @click="primeiro('Primeiro evento ativado!', $event), segundo('Segundo evento ativado!', $event)">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>

export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: ""
        }
    },
    methods: {
        primeiro(msg, e){
            this.multiplos_eventos = msg
        },
        segundo(msg, e){
            setTimeout(() => this.multiplos_eventos = msg, 500)
        }
    }
}
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>
