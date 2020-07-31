<template>

    <b-card :header="info.nombre" :img-src="info.logo" img-alt="Equipos" style="max-width: 20rem;" class="mb-2">
        <div class="card-text">
            Estado: 
            <div :class="{'activo': info.estado, 'inactivo': !info.estado}" class="circulo">
                
            </div>
            <br>
            Jugadores: {{ info.jugadores.length }}
        </div>
        <b-button href="#" variant="primary">Ver jugadores</b-button>
    </b-card>

</template>

<script>
export default {
    props: {
        info: {
            nombre: String,
            logo: String,
            estado: Boolean,
            jugadores: Array
        }
    },
    data() {
        return {
            
            // nombre: "Equipo 1",
            // logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            // estado: true,
            // jugadores: [{ jugador: "1" }, { jugador: "1" }, { jugador: "1" }]

        }
    }
}
</script>

<style scoped>
</style>