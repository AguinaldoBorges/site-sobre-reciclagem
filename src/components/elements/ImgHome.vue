<template>
  <div class="d-flex justify-content-center" >
    <img :src="img" id="img-home" />
  </div>
</template>

<script>
export default {
  props: {
    img: {}
  }

}
</script>

<style>
#img-home {
  width: 80%;
  height: 390px;
  border-radius: 25px;
  -webkit-animation: bounce-top 1.9s both;
	animation: bounce-top 1.9s both;
}

/* ANIMAÇÔES */
 @-webkit-keyframes bounce-top {
  0% {
    -webkit-transform: translateY(-45px);
            transform: translateY(-45px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
    opacity: 1;
  }
  24% {
    opacity: 1;
  }
  40% {
    -webkit-transform: translateY(-24px);
            transform: translateY(-24px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  65% {
    -webkit-transform: translateY(-12px);
            transform: translateY(-12px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  82% {
    -webkit-transform: translateY(-6px);
            transform: translateY(-6px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  93% {
    -webkit-transform: translateY(-4px);
            transform: translateY(-4px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  25%,
  55%,
  75%,
  87% {
    -webkit-transform: translateY(0px);
            transform: translateY(0px);
    -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
  }
  100% {
    -webkit-transform: translateY(0px);
            transform: translateY(0px);
    -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
    opacity: 1;
  }
}
@keyframes bounce-top {
  0% {
    -webkit-transform: translateY(-45px);
            transform: translateY(-45px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
    opacity: 1;
  }
  24% {
    opacity: 1;
  }
  40% {
    -webkit-transform: translateY(-24px);
            transform: translateY(-24px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  65% {
    -webkit-transform: translateY(-12px);
            transform: translateY(-12px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  82% {
    -webkit-transform: translateY(-6px);
            transform: translateY(-6px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  93% {
    -webkit-transform: translateY(-4px);
            transform: translateY(-4px);
    -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
  }
  25%,
  55%,
  75%,
  87% {
    -webkit-transform: translateY(0px);
            transform: translateY(0px);
    -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
  }
  100% {
    -webkit-transform: translateY(0px);
            transform: translateY(0px);
    -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
    opacity: 1;
  }
}

/* MEDIA QUERIES */

/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {
  /* Estilos aqui */
  #img-home {
    width: 100%;
    height: 350px;
    margin-top:15px;

  }
}

/* Estilos para dispositivos móveis de tela um pouco maior (480px) */
@media (min-width: 480px) {
  /* Estilos aqui */
  #img-home {
    width: 100%;
    height: 510px;
    margin-top:15px;


  }
}

/* Estilos para tablets e dispositivos móveis com tela maior (768px) */
@media (min-width: 768px) {
  /* Estilos aqui */
  #img-home {
    width: 100%;
    height: 400px;
  }
}

/* Estilos para laptops e monitores menores (992px) */
@media (min-width: 992px) {
  /* Estilos aqui */
  #img-home {
    width: 80%;
    height: 410px;
  }

}

/* Estilos para monitores maiores (1200px) */
@media (min-width: 1200px) {
  /* Estilos aqui */
  #img-home {
    width: 80%;
    height: 510px;
  }
}

</style>