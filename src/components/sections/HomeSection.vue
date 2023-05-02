<template>
    <div class="container-fluid" id="home-section">
        <!-- Logo -->
        <div class="row   p-5">
            <div class="col-md-6 col-sm-12">
                <img src="@/assets/logo.webp" id="home-logo" />
            </div>
            <div class="col-md-6 col-sm-12">
            </div>
        </div>

        <!-- Content -->
        <div class="row " id="home-content">
            <div class="col-md-6 col-sm-12 d-flex align-items-center p-4 pt-0 pb-0">
                <div class="row">
                    <TitleHome :text="'Bem vindos à nossa página sobre reciclagem! '" :color="'#CF1554'" />
                </div>
            </div>
            <div class="col-md-6 col-sm-12" >
                <ImgHome :img="require('../../assets/04-home.png')" />
            </div>
        </div>
    </div>
</template>

<script>
import TitleHome from '@/components/elements/TitleHome.vue'
import ImgHome from '@/components/elements/ImgHome.vue'

export default {
    components: {
        TitleHome,
        ImgHome,

    }
}
</script>

<style>
#home-section {
    /*background: url('@/assets/01-bg-home.jpg') no-repeat;
    background-size: cover;*/
    background-color: #7BED9F;
    min-height:calc(100vh - 50px);
}

#home-logo {
    width: 180px;
    display: block;
}

#home-content{
position: relative;
}

/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {
    /* Estilos aqui */
    #home-logo {
        width: 180px;
        display: none;
    }
    #home-section {
        /*background: url('@/assets/01-bg-home.jpg') no-repeat;
        background-size: cover;*/
        background-color: #7BED9F;
        min-height:calc(100vh - 50px);
    }
    #home-content{
        position: relative;
        top: -60px;
        }
  }

  /* Estilos para dispositivos móveis de tela um pouco maior (480px) */
  @media (min-width: 480px) {
    /* Estilos aqui */
    #home-logo {
        width: 180px;
        display: none;
    }
  }

  /* Estilos para tablets e dispositivos móveis com tela maior (768px) */
  @media (min-width: 768px) {
    /* Estilos aqui */
    #home-logo {
        width: 180px;
        display: none;
    }
  }

  /* Estilos para laptops e monitores menores (992px) */
  @media (min-width: 992px) {
    /* Estilos aqui */
    #home-logo {
        width: 180px;
        display: none;
    }

  }

  /* Estilos para monitores maiores (1200px) */
  @media (min-width: 1200px) {
    /* Estilos aqui */
    #home-logo {
        width: 180px;
        display: block;
    }

    #home-content{
        position: relative;
        top: -40px;
        }
  }
</style>