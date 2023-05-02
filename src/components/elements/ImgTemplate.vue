<template>
  <div class="d-flex justify-content-center" data-aos="fade-right" data-aos-duration="2000">
    <img :src="img" id="img-template" />
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
#img-template {
  width: 80%;
  height: 390px;
  border-radius: 25px;
}
/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {
  /* Estilos aqui */
  #img-template {
    width: 100%;
    height: 350px;
    margin-top:15px;

  }
}

/* Estilos para dispositivos móveis de tela um pouco maior (480px) */
@media (min-width: 480px) {
  /* Estilos aqui */
  #img-template {
    width: 100%;
    height: 350px;
    margin-top:15px;


  }
}

/* Estilos para tablets e dispositivos móveis com tela maior (768px) */
@media (min-width: 768px) {
  /* Estilos aqui */
  #img-template {
    width: 100%;
    height: 400px;
  }
}

/* Estilos para laptops e monitores menores (992px) */
@media (min-width: 992px) {
  /* Estilos aqui */
  #img-template {
    width: 80%;
    height: 410px;
  }

}

/* Estilos para monitores maiores (1200px) */
@media (min-width: 1200px) {
  /* Estilos aqui */
}

</style>