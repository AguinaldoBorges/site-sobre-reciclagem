<template>
  <div class="home container-fluid p-0 m-0">
    <div id="inicio" style="height:55px;" />
    <MenuTemplate id="menu-fixed" />
    <HomeSection />
    <div id="porque" style="position:relative; top:-55px;" />
    <AccountSection />
    <div id="quem_somos" style="position:relative; top:-55px;" />
    <AboutSection />
    <div id="videos" style="position:relative; top:-55px;" />
    <CardSection />
    <div id="contribuicao" style="position:relative; top:-55px;" />
    <LoanSection />
    <div id="fale-conosco" style="position:relative; top:-55px;" />
    <FooterSection />
    <a href="#inicio">
      <img :src="require('@/assets/10-voltar.png')" alt="seta para cima - voltar" id="back-top" />
    </a>
 </div>

</template>

<script>
// @ is an alias to /src

import MenuTemplate from '@/components/elements/MenuTemplate.vue';
import HomeSection from '@/components/sections/HomeSection.vue';
import AboutSection from '@/components/sections/AboutSection.vue';
import AccountSection from '@/components/sections/PorqueSection.vue';
import CardSection from '@/components/sections/VideosSection.vue';
import LoanSection from '@/components/sections/ContribuicaoSection.vue';
import FooterSection from '@/components/sections/FooterSection.vue';

export default {
  name: 'HomeView',
  components: {
    MenuTemplate,
    HomeSection,
    AboutSection,
    AccountSection,
    CardSection,
    LoanSection,
    FooterSection
  }
}
</script>
<style>
#back-top {
  background-color: #ffffffcb;
  width: 60px;
  padding: 3px;
  border-radius: 90px;
  position: fixed;
  bottom: 10px;
  right: 10px;
}

#menu-fixed {
  z-index: 2;
  position: fixed;
  top: 0;
  width: 100vw;
  background-color: #ffffff;

}


#section-home-space {
  height: 8px;
}

#back-top img {
  height: 55px;
  opacity: 70%;
}
</style>