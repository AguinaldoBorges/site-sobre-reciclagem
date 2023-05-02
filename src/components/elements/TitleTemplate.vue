<template>
    <div class="container-fluid">
      <!-- center -->
      <div class="row">
          <div class="col-12">
            <h1 id="title-template" :style="`color:${color}`">{{text}}<span :style="`color:${destakColor}`">{{destakText}}</span><span>{{text2}}</span></h1>
          </div>
      </div>
    </div>
  </template>

  <script>
  export default {
    props:{
        text:{},
        destakText:{},
        text2:{},
        color:{},
        destakColor:{}
    }

  }
  </script>

  <style>
  #title-template{
    font-weight: 700;
    font-size: 48px;
    text-shadow: -1px -1px 1px rgba(255,255,255,.1), 1px 1px 1px rgba(0,0,0,.5);
  }
/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {
  /* Estilos aqui */
  #title-template{
    font-weight: 900;
    font-size: 40px;
}
}

/* Estilos para dispositivos móveis de tela um pouco maior (480px) */
@media (min-width: 480px) {
  /* Estilos aqui */
  #title-template{
    font-weight: 900;
    font-size: 48px;
}
}

/* Estilos para tablets e dispositivos móveis com tela maior (768px) */
@media (min-width: 768px) {
  /* Estilos aqui */
  #title-template{
    font-weight: 900;
    font-size: 48px;
}
}

/* Estilos para laptops e monitores menores (992px) */
@media (min-width: 992px) {
  /* Estilos aqui */
  #title-template{
    font-weight: 900;
    font-size: 48px;
}

}

/* Estilos para monitores maiores (1200px) */
@media (min-width: 1200px) {
  /* Estilos aqui */
}
  </style>