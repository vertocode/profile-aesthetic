<template>
  <div id="services" class="mt-4 services">
    <h2 class="text-center title">Serviços</h2>
    <h3 class="text-center">Parcelamos qualquer procedimento a partir de R$100,00</h3>
    <div class="services-content mt-3">
      <div class="service" v-for="service in state.services" :key="service.title">
        <img :src="service.href" alt="Cílios" />
        <h3>{{ service.title }}</h3>
        <p>{{ service.description }}</p>
        <ul v-if="service?.prices">
          <li v-for="price in service?.prices" :key="price.title">{{ price.title }}: R${{ price.price.toFixed(2) }}</li>
        </ul>
      </div>
    </div>
    <div style="width: 100%; display: flex; justify-content: center; align-items: center; margin-bottom: 1rem">
      <a
        class="btn btn-success mb-3"
        style="color:white; width: 50rem; height: 3rem; background-color: rgb(180,168,185)"
        href="https://calendly.com/ericasleitao"
        target="_blank">
          Clique aqui para agendar o seu horário!
        </a>
    </div>
  </div>
</template>

<script setup>
import { reactive } from "vue";

const state = reactive({
  services: [
    {
      href: 'https://cdn.shopify.com/s/files/1/0570/3830/7506/articles/mulher-penteando-cilios_1.jpg?v=1636154392',
      title: 'Extensão de cílios',
      description: 'Oferecemos vários tipos de extensão de cílios, desde o mais natural até o mais dramático, com diferentes curvaturas, tamanhos e espessuras para atender às necessidades de cada cliente.',
      prices: [
        {
          title: 'Aplicacao Vol. Brasileiro',
          price: 120,
        },
        {
          title: 'Manutencao Vol. Brasileiro',
          price: 60,
        },
        {
          title: 'Aplicacao Vol. Egipcio 3D',
          price: 130,
        },
        {
          title: 'Manutencao Vol. Egipcio 3D',
          price: 60,
        },
        {
          title: 'Aplicacao Vol. Egipcio 4D',
          price: 140,
        },
        {
          title: 'Manutencao Vol. Egipcio 4D',
          price: 70,
        },
        {
          title: 'Aplicacao Vol. Arabe 5D',
          price: 150,
        },
        {
          title: 'Manutencao Vol. Arabe 5D',
          price: 70,
        },
        {
          title: 'Aplicacao Vol. Russo',
          price: 160,
        },
        {
          title: 'Manutencao Vol. Russo',
          price: 80,
        },
      ]
    },
    {
      href: 'https://galeriaglaser.com.br/wp-content/uploads/2018/11/glaser_blog01_outubro-e1577733833425.jpg',
      title: 'Design de Sobrancelhas',
      description: 'O nosso serviço de design de sobrancelha personalizado é uma oportunidade para você realçar a beleza natural dos seus olhos e obter sobrancelhas perfeitamente moldadas que harmonizam com os seus traços faciais.',
      prices: [
        {
          title: 'S/ hena',
          price: 25
        },
        {
          title: 'C/ hena',
          price: 25
        }
      ]
    },
    {
      href: 'https://www.depylaction.com.br/wp-content/uploads/2022/08/Linha-min-scaled.jpg',
      title: 'Epilacao Egipcia',
      description: 'A epilação egípcia, também conhecida como depilação com linha, é um método antigo e eficaz para remoção de pelos indesejados. Essa técnica milenar tem suas raízes no Egito e é amplamente utilizada até os dias de hoje devido aos seus resultados precisos e duradouros.',
      prices: [
        {
          title: 'buco',
          price: 10
        },
        {
          title: 'completa',
          price: 20
        }
      ]
    },
    {
      href: 'https://images.squarespace-cdn.com/content/v1/60d0ed1735327e5ca356494b/1628766485150-PMEXKYAVW8NLQQEYY273/tratamento-para-calvice.jpg',
      title: 'Tratamento Capilar',
      description: 'A queda de cabelo é um problema que afeta muitas pessoas e pode ter várias causas, como genética, estresse, alterações hormonais, entre outras. No ramo da estética, existem diversos tratamentos que podem ajudar a combater a queda de cabelo e promover o crescimento saudável dos fios.',
      prices: [
        {
          title: 'Detox Capilar + Massagem Craniana',
          price: 100
        },
        {
          title: 'Microagulhamento',
          price: 199.99
        },
        {
          title: 'Detox Capilar + Massagem Craniana + Microagulhamento',
          price: 250
        }
      ]
    },
    {
      href: 'https://static.wixstatic.com/media/a6fb2b_d77d5c36b3be4db5a98ce0b3fa1e311b~mv2.png/v1/fill/w_640,h_334,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/a6fb2b_d77d5c36b3be4db5a98ce0b3fa1e311b~mv2.png',
      title: 'Curso de extensão de cílios',
      description: 'Nosso curso de extensão de cílios é projetado para profissionais que desejam aprimorar suas habilidades e se tornarem especialistas em técnicas de alongamento de cílios.',
      prices: [
        {
          title: 'Lash iniciante',
          price: 999.99
        }
      ]
    }
  ]
})
</script>

<style>
.services {
  margin: auto;
  width: 100%;
}

.services-content {
  width: 100%;
  display: flex;
  gap: 50px;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: baseline;
  margin: 0 auto;
  max-width: 1200px;
}

.service {
  width: 20em;
  margin-bottom: 30px;
}

.service img {
  width: 100%;
  height: 10em;
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
