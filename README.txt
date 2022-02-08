
gradientes / transformaciones / animaciones
-----------------------------------------------------------

/* amplia fotos de productos 20% con :hover*/
.contFotoProduc:hover { 
   transform: scale(1.2);
   transition: 1.5s;
 }
-------------------------------------------------------------
/*genera gradiente lineal en el body*/
body {
  /* background-color: ##f29f04; */
  background-image: linear-gradient( 135deg, #f22222 50%, #f29f04);
}
-------------------------------------------------------------
/*acceso cambia de color al presionar click */
nav a:active {
  color: #f22222}
--------------------------------------------------------------
/*acceso se amplia al pasar el mouse*/
nav li:hover {
  transform: scale(1.5);
  transition: 1s;
}
--------------------------------------------------------------
/*rotacion animada del logo*/
.logo {
   position: absolute;
   margin-top: 15px;
   margin-left: 15px;
   animation-name: movimiento;
   animation-duration: 3s;
   animation-iteration-count: 2;
   animation-direction: alternate;
 }

 @keyframes movimiento {
   0% {
     transform: rotate(0deg);
   }
   100% {
     transform: rotate(360deg);
   }
 }
----------------------------------------------------------
/*pausa animación al pasar el puntero*/
  .logo:hover{
    animation-play-state: paused;
  }

