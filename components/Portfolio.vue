<template>
  <main id="portfolio">
    <h2 class="text-center title">Portfolio</h2>
    <div class="volume">
      <h3>Volume Brasileiro:</h3>
      <Slider :images="volBr" style="margin: auto; width: 100%"/>
    </div>

    <div class="volume">
      <h3>Volume Egipcio:</h3>
      <Slider :images="volEg" style="margin: auto; width: 100%"/>
    </div>

    <div class="volume">
      <h3>Volume Russo:</h3>
      <Slider :images="volRs" style="margin: auto; width: 100%"/>
    </div>
  </main>

</template>
<script setup>

import Slider from "~/components/slider/Slider.vue";

const volBr = [
  {image: 'https://www.gaz.com.br/uploads/2022/06/P3-2-Brasileiro.jpg'},
  {image: 'https://cdn.sistemawbuy.com.br/arquivos/e82e7997317d0a500738e3499f96ce88/produtos/JE6SA3/volume-brasileiro-63ed2dfee669f.jpg'},
  {image: 'https://blog.meninashoes.com.br/wp-content/uploads/2023/01/extensao-de-cilios-volume-egipcio-maos-de-fada-1-1024x943.jpg'},
  {image: 'https://florisbellaesmalteria.com.br/wp-content/uploads/2023/03/extensao-de-cilios-volume-brasileiro-manutencao-v1.jpg'}
]

const volEg = [
  {image: 'https://cf.shopee.com.br/file/e2e218b053794e2027e7eea0a259109b'},
  {image: 'https://i.pinimg.com/736x/79/29/01/792901b763f093fec0f3ecbacb88db73.jpg'},
  {image: 'https://www.cidadeoferta.com.br/storage/offers/6534-nubia-gumiero-lash-designer-londrina-extensao-de-cilios-imagem-2.jpg'}
]

const volRs = [
  {image: 'https://blog.meninashoes.com.br/wp-content/uploads/2023/01/extensao-de-cilios-mega-volume-karla_uselash.jpg'},
  {image: 'https://img.olx.com.br/images/52/524366275620539.jpg'}
]
</script>

<style scoped>
h3 {
  text-align: center;
  font-family: Roboto,sans-serif ;
}

.volume {
  margin-top: 3rem;
}
</style>

