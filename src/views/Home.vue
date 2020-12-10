<template>
<div class="padre fondoprincipal">
  <div class="diseño1">
    <button class="bonitoboton bttn-inicio fondobotones" type="submit" @click="siguiente()"><h2><p>JUEGO RAPIDO</p></h2></button>
  </div>
</div>
</template>

<script>

export default {
  name: 'Home',
  mounted(){
    localStorage.clear();

  },
  methods: {
        siguiente(){
            localStorage.setItem('categoria', this.cat);
            this.$router.push("/Categorias")
        }
    }
}
</script>
