<template>
    <div class="container-fluid" id="quem-somos-section">
        <!-- Content -->
        <div class="row  d-flex align-items-center pt-5 pb-5" id="about-row">
            <div class="col-12 d-flex text-center justify-content-center" style="padding-left:30px;">
                <h2 class="">
                    <TitleTemplate :text="'Quem somos '" :color="'#CF1554'" :destakText="''" :destakColor="'#7BED9F'"
                        :text2="''" class="section-one-text-container" />
                    <TextTemplate
                        :text="'Estudantes de Pedagogia pela Faculdade Flamingo, tivemos como objetivo construir um puxa saco, uma palmeira e uma lixeira a partir de garrafas pet`s, a fim de mostrar a importância da reciclagem e da separação correta do lixo, conforme proposto pela disciplina de Metodologia de Ensino das Ciências Naturais. Nosso grupo é formado por: '"
                        :color="'#252525'" class="pt-3 section-one-text-container" />
                </h2>
            </div>
            <div class="col-lg-3 col-md-6 col-sm-12 d-flex text-center justify-content-center" v-for="aluna in alunas"
                :key="aluna.index">
                <div class="card text-center mb-3" style="width: 99%;">
                    <div class="card-body">
                        <img :src="aluna.foto" alt="foto da integrante do grupo" class="card-image" />
                        <h5 class="card-title">{{ aluna.nome }}</h5>
                        <p class="card-text">{{ aluna.ra }}</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
import TitleTemplate from '@/components/elements/TitleTemplate.vue'
import TextTemplate from '@/components/elements/TextTemplate.vue'
export default {
    components: {
        TitleTemplate,
        TextTemplate
    },
    data() {
        return {
            alunas: [
                {
                    nome: 'Fernanda Pereira Santos',
                    ra: 'RA: 22207875',
                    foto: require('@/assets/3.png')
                },
                {
                    nome: 'Ingrid de Carvalho de Souza',
                    ra: 'RA: 18203639',
                    foto: require('@/assets/2.png')
                },
                {
                    nome: 'Letícia Ap. G. de A. S. R. Borges',
                    ra: 'RA: 22107690',
                    foto: require('@/assets/4.png')
                },
                {
                    nome: 'Sabrina Ferreira Maximiano',
                    ra: 'RA: 22207865',
                    foto: require('@/assets/1.png')
                }
            ]
        }
    },
}
</script>

<style>
#quem-somos-section {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #cf295528;
    min-height: 100vh;
    width: 100vw;
    padding-left: 0%;
    padding-right: 0%;
    margin: 0%;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

#about-row {
    min-height: 100vh;

}

.about-text-container {
    padding: 0 70px;
    padding-left: 15px;
}

.card {
    -webkit-box-shadow: 0px 10px 13px -7px #000000, -50px -50px 0px -29px rgba(0, 0, 0, 0);
    box-shadow: 0px 10px 13px -7px #000000, -50px -50px 0px -29px rgba(0, 0, 0, 0);
}

.card :hover {
    background-color: #7BED9F;
    color: #252525;
}

.card-image {
    width: 250px;
}

.card-title {
    color: #cf2954;
}</style>