<template>
    <div class="container-fluid" id="footer-section">
        <!-- Content -->
        <div class="row pt-5 pb-5">
            <div class="col-md-6 col-sm-12">
                <img src="@/assets/logo.webp" id="footer-logo" />
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12" id="footer-content">
                <TitleTemplate :text="'Fale com o desenvolvedor'" :color="'#CF1554'" />
                <TextTemplate
                    :text="'Entre em contato se tiver alguma idéia que queira colocar na web. Deixe-me dar vida à suas idéias! Estarei sempre aqui para ajudar.'"
                    :color="'#252525'" />
                <TextTemplate :text="'Email: tiaguinaldo2017@gmail.com'" :color="'#CF1554'" />
                <TextTemplate :text="'Whatsapp: (11) 99015 3359'" :color="'#CF1554'" />

            </div>
        </div>
        <!-- Copyrights -->
        <div class="row " id="footer-copyrights">
            <TextTemplate :text="'Copyright © 2023 '" :color="'#ffffff'" :destakText="'Aguinaldo Borges.'"
                :destakColor="'#252525'" :text2="' Todos os direitos reservados.'" />
        </div>
    </div>
</template>

<script>
import TitleTemplate from '@/components/elements/TitleTemplate.vue'
import TextTemplate from '@/components/elements/TextTemplate.vue'
export default {
    components: {
        TitleTemplate,
        TextTemplate,

    }
}
</script>

<style>
#footer-section {
    /*'background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #7BED9F;
    width: 100vw;
    min-height: 100vh;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

#footer-logo {
    display: block;
    width: 180px;
}

#footer-content {
    min-height: 350px;
    position: relative;
    left: -6px;

}

#footer-copyrights {
    text-align: center;
    position: relative;
    bottom: -70px;
    align-items: flex-end;
    height: 50px;
    margin: 0;
    padding-left: 15px;
}

#footer-text {
    text-align: left;
}

/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {

    /* Estilos aqui */
    #footer-logo {
        display: none;
    }

    #footer-text {
        text-align: center;
    }

    #footer-content {


    }

    #footer-copyrights {
        position: relative;
        top: -40px;
    }
}

/* Estilos para dispositivos móveis de tela um pouco maior (480px) */
@media (min-width: 480px) {

    /* Estilos aqui */
    #footer-logo {
        display: none;
    }

    #footer-text {
        text-align: left;
    }

    #footer-content {
        position: relative;
        top: -12%;

        margin-left: -7px;
    }

    #footer-copyrights {
        position: relative;
        top: 0px;

    }
}

/* Estilos para tablets e dispositivos móveis com tela maior (768px) */
@media (min-width: 768px) {

    /* Estilos aqui */
    #footer-logo {
        display: none;
    }

    #footer-text {
        text-align: center;
    }

    #footer-content {
        position: relative;
        top: 0;
        padding: 0 80px;
    }

    #footer-copyrights {
        position: relative;
        top: 0px;
    }
}

/* Estilos para laptops e monitores menores (992px) */
@media (min-width: 992px) {

    /* Estilos aqui */
    #footer-logo {
        display: block;
    }

    #footer-text {
        text-align: left;
    }

    #footer-content {
        position: relative;
        top: 10%;
    }

    #footer-copyrights {
        position: relative;
        top: 0px;
    }

}

/* Estilos para monitores maiores (1200px) */
@media (min-width: 1200px) {

    /* Estilos aqui */
    #footer-logo {
        display: block;
    }

    #footer-text {
        text-align: left;
    }

    #footer-content {
        position: relative;
        top: 10%;
    }

    #footer-copyrights {
        position: relative;
        top: 0px;
        padding-left: 40px;
    }
}
</style>