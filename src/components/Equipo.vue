<template>

    <b-card :header="nombre" :img-src="logo" img-alt="Equipos" style="max-width: 20rem;" class="mb-2">
        <p class="card-text">
            Estado: 
            <div :class="{'activo': estado, 'inactivo': !estado}" class="circulo">
                
            </div>
            <br>
            Jugadores: {{ jugadores.length }}
        </p>
        <b-button href="#" variant="primary">Ver jugadores</b-button>
    </b-card>

</template>

<script>
export default {
    data() {
        return {

            nombre: "Equipo 1",
            logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            estado: true,
            jugadores: [{ jugador: "1" }, { jugador: "1" }, { jugador: "1" }]

        }
    }
}
</script>

<style scoped>
</style>