<template>
    <div class="container-fluid">
        <nav class="navbar navbar-expand-lg col" id="menu-navbar">
            <div class="container-fluid">
                <a class="navbar-brand" href="#home-top">
                    <img src="@/assets/logo.webp" alt="Bootstrap" width="120" height="24">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                    aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item" v-for="item in menuItens" :key="item.index">
                            <a class="nav-link active" aria-current="page" :href="item.url"><span class="text-menu">{{item.label}}</span></a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    data() {
        return {
            menuItens:[
                {
                    label:'Home',
                    url:'#inicio'
                },
                {
                    label:'Por que reciclar',
                    url:'#porque'
                },
                {
                    label:'Quem somos',
                    url:'#quem_somos'
                },

                {
                    label:'Faça você mesmo',
                    url:'#videos'
                },
                {
                    label:'Contribuição',
                    url:'#contribuicao'
                },
                {
                    label:'Fale conosco',
                    url:'#fale-conosco'
                },
            ]
        }
    },
}
</script>

<style>
#menu-tudo{
    background-color: #dbb60ebd;
}
#menu-navbar{
    background-color: #ffffff;
    text-align: center;
}

.text-menu{
    font-size: 20px;
    font-weight: 500;
    color: #CF2954;
}

/* Estilos para dispositivos móveis pequenos (320px) */
@media (min-width: 320px) {
    /* Estilos aqui */

  }

  /* Estilos para dispositivos móveis de tela um pouco maior (480px) */
  @media (min-width: 480px) {
    /* Estilos aqui */

  }

  /* Estilos para tablets e dispositivos móveis com tela maior (768px) */
  @media (min-width: 768px) {
    /* Estilos aqui */

  }

  /* Estilos para laptops e monitores menores (992px) */
  @media (min-width: 992px) {
    /* Estilos aqui */

  }

  /* Estilos para monitores maiores (1200px) */
  @media (min-width: 1200px) {
    /* Estilos aqui */
  }
</style>