<template>
  <div id="about-me" class="about-me mt-4">
    <h2 class="text-center title">Ola, Seja muito bem vinda garotas!</h2>
    <main class="content p-5">
      <div>
        <p>Eu sou uma esteticista apaixonada pela minha profissão e pelo bem-estar dos meus clientes. Com anos de experiência em tratamentos faciais, corporais e de beleza em geral, estou comprometida em oferecer serviços de alta qualidade, utilizando as técnicas mais avançadas e os melhores produtos disponíveis no mercado.</p>
        <p>Acredito que cada pessoa é única e, por isso, adapto meus tratamentos às necessidades individuais de cada cliente, garantindo que cada um se sinta cuidado e mimado em minha clínica. Além disso, estou sempre atualizada com as últimas tendências e tecnologias do setor de beleza, para oferecer aos meus clientes o melhor que a estética tem a oferecer.</p>
        <p>Para mim, não se trata apenas de cuidar da aparência externa, mas de promover uma sensação de bem-estar e autoconfiança em meus clientes, para que eles possam se sentir bem consigo mesmos por dentro e por fora. Estou ansiosa para recebê-lo em minha clínica e ajudá-lo a alcançar a melhor versão de si mesmo!</p>
      </div>
      <aside>
        <img src="https://i.imgur.com/AOF0s3m.jpg" alt="Foto da Erica">
      </aside>
    </main>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.about-me {
  background-color:#eee;
  margin: auto 50px;
  width: 90%;
}

.content {
  height: 70vh;
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

.content img {
  width: 500px;
  height: 500px;
  border-radius: 100%;
  object-fit: cover;
  object-position: center;
}

</style>
