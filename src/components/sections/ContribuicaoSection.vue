<template>
    <div class="container-fluid d-flex align-items-center" id="contribuicao-section">
        <!-- Content -->
        <div class="row   pt-5 pb-5">
            <div class="col-md-6 col-sm-12 p-0">
                <TitleTemplate :text="'Contribuição'" :color="'#CF1554'" class="col-12" />
                    <TextTemplate :text="'Ao reaproveitar '" :color="'#252525'" :destakText="'garrafas pet`s'" :destakColor="'#CF1554'" :text2="' para criar objetos como os que propomos, estamos contribuindo para poupar o meio ambiente dessa decomposição, que pode levar de 450 a 500 anos para ocorrer. Além disso, estamos ajudando a diminuir o consumo do plástico, um material que demora muito tempo para se decompor e é responsável por grande parte da poluição presente nos oceanos e em outros ecossistemas.'" class="col-12" />
                    <TextTemplate :text="'O meio ambiente agradece!'" :color="'#252525'" class="col-12" />
                <div class="row">


                </div>
            </div>
            <div class="col-md-6 col-sm-12 mt-4">
                <ImgTemplate :img="require('../../assets/09-loan-section.png')" />
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
#contribuicao-section {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #ffffff;
    min-height: 100vh;
    width: 100vw;
    padding-left: 25px;
    padding-right: 0px;
}

</style>