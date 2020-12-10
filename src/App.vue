<template>
  
  <router-view/>
</template>

<style>
*{
  margin: 0;
  padding: 0;
  text-decoration: none;
  box-sizing: border-box;
}
.centrar{
  text-align: center;
}
/* swal */
.swal-overlay {
  background-color: rgba(0, 0, 0, 0.8);
}
.swal-modal {
  background-color: rgb(0, 255, 21);
  border: 3px solid rgb(255, 255, 255);
}
.swal-title {
  margin: 0px;
  font-size: 18px;
  margin-bottom: 28px;
  color: rgb(0, 0, 0);
  text-transform: uppercase;
}
.swal-text{
  color: black;
}
.swal-footer {
  background-color: rgb(245, 248, 250);
  margin-top: 32px;
  border-top: 1px solid #bac2c7;
  overflow: hidden;
  text-align: center;
}
.swal-button {
  padding: 10px 19px;
  border-radius: 5px;
  font-size: 12px;
  border: 1px solid #000000;
  text-shadow: 0px -1px 0px rgba(0, 0, 0, 0.3);
  color: rgb(255, 255, 255);
}
.swal-button--reiniciar{
  background-color: #1fff50,
}
.swal-button--home {
  background-color: rgba(59, 38, 252, 0.952);
}
/*fondos*/
.fondoprincipal{
  background: url('assets/fondo/fondo4.jpg');
}
.fondobotones{
  background: url('assets/fondo/fondo5.jpg');
}
/*fondo final*/
.fondofinal{
  background: url('assets/fondo/fondo6.jpg');
}
/*centrado*/
.padre{
  background-size: 135%;
  text-align: center;
  width: 100%;
  height: 100vh;
  display: table;
}
.diseño1{
  display: table-cell;
  vertical-align: middle;
}
.diseño2{
  width: 50%;
  padding: 3px 3px 3px 5px;

  display: inline-block;
}
/* imagen */
.estilotarjeta{
  padding: auto;
  width: 100%;
  height: auto;
  height: 25vh;
  border-radius: 15px;
  border-style: solid;
  border-color: rgb(18, 20, 60);
}
img.card-img-top.girar {
    animation: fadein 2s;
}

@keyframes fadein {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}
/*BOTONES BONITOS*/
.bonitoboton{
  background-size: 100%;
  display: block;
  padding: 10px;
  text-align: center;
  margin: auto;
  border-color: black;
  border-width: 2px;
  font-family: 'Algerian Black';

  border-radius: 10px;
  width: 98%;
  height: 70px;
  font-size: small;

  text-transform: uppercase;
  border-radius: 20px;
  width: 100%;
  height: 70px;
  font-size: 18px;
}
.imagenboton{
  width: 30px;
  height: 30px;
}
.bttn:hover{
  transform: translateY(5px);
  box-shadow: 0px 30px 5px -15px rgba(0,0,0,0.3);
}
</style>
