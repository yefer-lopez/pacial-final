<template>
    <div class="categorias padre fondoprincipal">
        <div class="diseño1">
            <div class="diseño2">
                <button class="bonitoboton bttn-cat fondobotones" type="submit" v-on:click="cat='animales'" @click="siguiente()"><h2>Animales</h2></button>
            </div>
            <div class="diseño2">
                <button class="bonitoboton bttn-cat fondobotones" type="submit" v-on:click="cat='frutas'" @click="siguiente()"><h2>Frutas</h2></button>
            </div>
            <br>
            <div class="diseño2">
                <button class="bonitoboton bttn-cat fondobotones" type="submit" v-on:click="cat='paisajes'" @click="siguiente()"><h2>Paisajes</h2></button>
            </div>
            <div class="diseño2">
                <button class="bonitoboton bttn-cat fondobotones" type="submit" v-on:click="cat='deportes'" @click="siguiente()"><h2>Deportes</h2></button>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    name: 'Categorias',
    data(){
        return{
            cat: '',
        }
    },
    mounted(){
        localStorage.removeItem("categoria")
    },
    methods: {
        siguiente(){
            localStorage.setItem('categoria', this.cat);
            this.$router.push("/Cuadriculas")
        }
    }
}

</script>