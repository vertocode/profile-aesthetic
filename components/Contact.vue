<template>
  <main id="contact">
    <h2 class="text-center title">Contato</h2>
    <div class="contact-card">
      <div class="contact-card-body">
        <h2>Entre em Contato</h2>
        <p class="card-description">Estamos aqui para cuidar de você. Entre em contato para agendar um tratamento relaxante e rejuvenescedor.</p>
        <div class="contact-links">
          <a class="instagram-link" href="https://www.instagram.com/herica_estetica" target="_blank">
            <i class="fab fa-instagram"></i> Instagram
          </a>
          <a class="whatsapp-link" href="https://api.whatsapp.com/send?phone=5535984597781&text=Vim%20pelo%20site,%20gostaria%20de%20agendar%20um%20hor%C3%A1rio!" target="_blank">
            <i class="fab fa-whatsapp"></i> WhatsApp
          </a>
          <a class="schedule-link" href="https://calendly.com/ericasleitao">
            <i class="far fa-calendar-alt"></i> Agende Agora
          </a>
        </div>
      </div>
    </div>
  </main>
</template>

<style>
.contact-card {
  margin: 2em auto;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
  padding: 20px;
  max-width: 400px;
  width: 100%;
}

.contact-card-body {
  text-align: center;
}

.contact-links a {
  cursor: pointer;
  display: inline-block;
  margin: 10px;
  padding: 10px 20px;
  color: #fff;
  border-radius: 5px;
  text-decoration: none;
}

.instagram-link {
  background-color: #e4405f;
}

.whatsapp-link {
  background-color: #25d366;
}

.schedule-link {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  color: #fff;
  background-color: #007bff;
  border-radius: 5px;
  text-decoration: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.schedule-link i {
  margin-right: 8px;
}

.schedule-link:hover {
  background-color: #0056b3;
}

.card-description {
  font-size: 14px;
  color: #555;
  margin-bottom: 20px;
}
</style>

<script setup lang="ts">
import '@fortawesome/fontawesome-free/css/all.css'
</script>
