<template>
    <div class="categorias padre fondoprincipal">
        <div class="diseño1">
            <div class="diseño2">
                <button class="bonitoboton fondobotones " type="submit" v-on:click="ancho=2,largo=3" @click="siguiente()"><h2>3x2</h2></button>
            </div>
            <div class="diseño2">
                <button class="bonitoboton fondobotones " type="submit" v-on:click="ancho=3,largo=4" @click="siguiente()"><h2>4x3</h2></button>
            </div>
            <br>
            <div class="diseño2">
                <button class="bonitoboton fondobotones" type="submit" v-on:click="ancho=4,largo=5" @click="siguiente()"><h2>5x4</h2></button>
            </div>
            <div class="diseño2">
                <button class="bonitoboton fondobotones" type="submit" v-on:click="ancho=5,largo=6" @click="siguiente()"><h2>6x5</h2></button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Cuadriculas',
    data(){
        return{
            ancho: 0,
            largo: 0
        }
    },
    mounted(){
        localStorage.removeItem("largo")
        localStorage.removeItem("ancho")
        if (localStorage.getItem('categoria') === null) {
            this.$router.push("/Categorias")
        }
    },
    methods: {
        siguiente(){
            localStorage.setItem('largo', this.largo);
            localStorage.setItem('ancho', this.ancho);
            this.$router.push("/Juego")
        }
    }
}
</script>