<template>
    <div class="container-fluid " id="videos-section">
        <!-- Video 1 -->
        <div class="row pt-5 pb-5" id="video1">
            <div class="col-md-6 col-sm-12">
                <iframe width="100%" height="100%" :src="videos[0].link" :title="videos[0].label"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen></iframe>
            </div>
            <div class="col-md-6 col-sm-12 d-flex align-items-center mt-4">
                <div class="row">
                    <TitleTemplate :text="videos[0].label" :color="'#CF1554'" class="col-12" />
                    <TextTemplate :text="videos[0].description"
                        :color="'#252525'" :destakText="''" :destakColor="'#CF1554'" class="col-12" />
                </div>
            </div>
        </div>
        <!-- Video 2 -->
        <div class="row pt-5 pb-5" id="video2">
            <div class="col-md-6 col-sm-12 d-flex align-items-center mt-4">
                <div class="row">
                    <TitleTemplate :text="videos[1].label" :color="'#CF1554'" class="col-12" />
                    <TextTemplate :text="videos[1].description"
                        :color="'#252525'" :destakText="''" :destakColor="'#CF1554'" class="col-12" />
                </div>
            </div>
            <div class="col-md-6 col-sm-12">
                <iframe width="100%" height="100%" :src="videos[1].link" :title="videos[1].label"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen></iframe>
            </div>
        </div>
        <!-- Video 3 -->
        <div class="row pt-5 pb-5" id="video3">
            <div class="col-md-6 col-sm-12">
                <iframe width="100%" height="100%" :src="videos[2].link" :title="videos[2].label"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen></iframe>
            </div>
            <div class="col-md-6 col-sm-12 d-flex align-items-center mt-4">
                <div class="row">
                    <TitleTemplate :text="videos[2].label" :color="'#CF1554'" class="col-12" />
                    <TextTemplate :text="videos[2].description"
                        :color="'#252525'" :destakText="''" :destakColor="'#CF1554'" class="col-12" />
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
            videoLink: 'https://www.youtube.com/embed/sWd_uktmOiw',
            videos: [
                {
                    label: 'Puxa saco',
                    description:'Aprenda fazer um incrível Puxa Saco recilável, sem costura, usando garrafa pet!',
                    icone: require('@/assets/puxa-saco.png'),
                    link: 'https://www.youtube.com/embed/DzoNMDRpmUA',
                },
                {
                    label: 'Palmeira',
                    description:`Neste vídeo você vai aprender fazer uma linda palmeira para enfeitar sua casa ou presentear alguem. E o melhor: Reciclável, usando garrafa pet!`,
                    icone: require('@/assets/palmeira.png'),
                    link: 'https://www.youtube.com/embed/gI-1Z73MhFM',
                },
                {
                    label: 'Lixeira',
                    description:'Lugar de Lixo é no Lixo. Aprenda a fazer essa maravilhosa lixeira de garrafa pet, totalmente reciclável!',
                    icone: require('@/assets/cesto.png'),
                    link: 'https://www.youtube.com/embed/sWd_uktmOiw',
                },
            ]
        }
    },
    methods: {
        changeVideo(link) {
            this.videoLink = link
        }
    }
}
</script>

<style>
#videos-section {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #ffffff;
    min-height: 100vh;
    padding-left: 0%;
    padding-right: 0%;
    margin: 0%;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;


}
#video1 {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #7BED9F;
    min-height: 100vh;
    width: 100%;
}
#video1 iframe {
    -webkit-box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
    box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
}
#video2 {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #ffffff;
    min-height: 100vh;
    width: 100vw;
}
#video2 iframe {
    -webkit-box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
    box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
}
#video3 {
    /*background: url('@/assets/02-bg-section.jpg') no-repeat;
    background-size: cover;*/
    background-color: #cf295528;
    min-height: 100vh;
    width: 100vw;
}
#video3 iframe {
    -webkit-box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
    box-shadow: 8px 0px 0px 0px #DCD0C0, 0px 8px 0px 0px #DA635D, -8px 0px 0px 0px #4E4E56, 0px 0px 0px 8px #cf2954, 5px 5px 15px 5px rgba(0,0,0,0);
}
</style>