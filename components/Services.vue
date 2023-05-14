<template>
  <div id="services" class="mt-4 services">
    <h2 class="text-center title">Meus serviços de estética</h2>
    <div class="services-content p-5">
      <div class="service" v-for="service in state.services" :key="service.title">
        <img :src="service.href" alt="Cílios" />
        <h3>{{ service.title }}</h3>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { reactive } from "vue";

const state = reactive({
  services: [
    {
      href: 'https://cdn.shopify.com/s/files/1/0570/3830/7506/articles/mulher-penteando-cilios_1.jpg?v=1636154392',
      title: 'Cílios',
      description: 'Oferecemos vários tipos de extensão de cílios, desde o mais natural até o mais dramático, com diferentes curvaturas, tamanhos e espessuras para atender às necessidades de cada cliente.'
    },
    {
      href: 'https://images.squarespace-cdn.com/content/v1/60d0ed1735327e5ca356494b/1628766485150-PMEXKYAVW8NLQQEYY273/tratamento-para-calvice.jpg',
      title: 'Tratamento Capilar contra queda',
      description: 'A queda de cabelo é um problema que afeta muitas pessoas e pode ter várias causas, como genética, estresse, alterações hormonais, entre outras. No ramo da estética, existem diversos tratamentos que podem ajudar a combater a queda de cabelo e promover o crescimento saudável dos fios.'
    }
  ]
})
</script>

<style>
.services {
  margin: auto 50px;
  width: 90%;
  background-color:#eee;
}
.services-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: baseline;
  margin: 0 auto;
  max-width: 1200px;
}

.service {
  width: 30%;
  margin-bottom: 30px;
}

.service img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 10px;
}

.service h3 {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.service p {
  font-size: 16px;
  line-height: 1.4;
  margin-bottom: 0;
}
</style>
