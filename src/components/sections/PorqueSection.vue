<template>
    <div class="container-fluid d-flex align-items-center" id="porque-section">
        <!-- Content -->
        <div class="row">
            <div class="col-md-6 col-sm-12 d-flex align-items-center justify-content-center">
                <div class="row ">
                    <TitleTemplate :text="'Por que a reciclagem é importante? '" :color="'#CF1554'" class="col-12" />
                    <TextTemplate :text="'Além de ajudar a preservar o meio ambiente, ela contribui para a diminuição da quantidade de resíduos que são depositados em aterros sanitários e lixões. Para que a reciclagem seja efetiva, é fundamental que a população faça a separação correta dos materiais recicláveis, seguindo as orientações dos programas de coleta seletiva. '" :color="'#252525'" class="col-12" />
                </div>
            </div>
            <div class="col-md-6 col-sm-12 mt-4">
                <ImgTemplate :img="require('../../assets/07-account-section.jpg')" />
            </div>
        </div>
    </div>
</template>

<script>
import TitleTemplate from '@/components/elements/TitleTemplate.vue'
import TextTemplate from '@/components/elements/TextTemplate.vue'
import ImgTemplate from '@/components/elements/ImgTemplate.vue'
export default {
    components: {
        TitleTemplate,
        TextTemplate,
        ImgTemplate,
    }
}
</script>

<style>
#porque-section {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #ffffff;
    padding-top: 35px;
    padding-bottom: 35px;
    min-height: 100vh;
    width: 100vw;
    padding-left: 0%;
    padding-right: 0%;
    margin: 0%;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

</style>