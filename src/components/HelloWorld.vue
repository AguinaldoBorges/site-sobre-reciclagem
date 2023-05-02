<template>
  <div>
    <MenuTemplate/>
    <div class="hello container">
      <!-- layout -->
      <div class="row bg-primary  mt-4">
        <div class="col-12">
          <TitleTemplate :text="'LAYOUT'" :color="'#ffffff'"/>
        </div>
      </div>

      <!-- center -->
      <div class="row bg-dark text-light ">
        <div class="col-12">
          <TitleTemplate :text="'Título Centralizado'"/>
          <TextTemplate :text="'Texto Centralizado'"/>
        </div>
      </div>

      <!-- image right -->
      <div class="row bg-dark text-light ">
        <div class="col-md-6 col-sm-12">
          <TextTemplate :text="'Texto'"/>
        </div>
        <div class="bg-light text-dark col-md-6 col-sm-12">
          imagem
        </div>
      </div>

      <!-- image left -->
      <div class="row">
        <div class="bg-light text-dark col-md-6 col-sm-12">
          imagem
        </div>
        <div class="bg-dark text-light col-md-6 col-sm-12">
          <TextTemplate :text="'Texto'"/>
        </div>
      </div>

      <!-- COMPONENTES -->
      <div class="row mt-4">
        <div class="bg-primary col-12">
          <TitleTemplate :text="'COMPONENTES'" :color="'#ffffff'"/>
        </div>
      </div>

      <!-- Textos -->
      <div class="row bg-dark text-light ">
        <div class="col-12">
          <TitleHome  :text="'Bem '" :color="'#ffffff'" :destakText="'vindo'" :destakColor="'#9340FF'"  :text2="' ao DuckBank!'"/>
          <TitleTemplate :text="'Bem '" :color="'#ffffff'" :destakText="'vindo'" :destakColor="'#9340FF'"  :text2="' ao DuckBank!'"/>
          <TextTemplate :text="'Bem '" :color="'#ffffff'" :destakText="'vindo'" :destakColor="'#9340FF'"  :text2="' ao DuckBank!'"/>
        </div>
      </div>

      <!-- Imagens -->
      <div class="row bg-dark text-light ">
        <div class="col-12">
          <ImgTemplate :img="require('@/assets/04-home.jpg')"/>
        </div>
      </div>

      <!-- Buttons -->
      <div class="row bg-dark text-light p-4">
        <div class="col-12">
          <BtnTemplate :text="'Saiba mais'"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TitleHome from '../components/elements/TitleHome.vue';
import TitleTemplate from '../components/elements/TitleTemplate.vue';
import TextTemplate from '../components/elements/TextTemplate.vue';
import ImgTemplate from '../components/elements/ImgTemplate.vue';
import BtnTemplate from '../components/elements/BtnTemplate.vue';
import MenuTemplate from '../components/elements/MenuTemplate.vue';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components:{
    TitleHome,
    TitleTemplate,
    TextTemplate,
    ImgTemplate,
    BtnTemplate,
    MenuTemplate
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#colors{
  /*title*/
  color:#9340FF;
  /*background*/
  color:#101728;
  /*text*/
  color:#FFFFFF;

}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
