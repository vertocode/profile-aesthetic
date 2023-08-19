<template>
  <div>
    <header>
      <div class="header-content">
        <h1>Érica</h1>
        <button class="menu-toggle" @click="toggleMenu">
          <i class="fas fa-bars"></i>
        </button>
      </div>
    </header>
    <nav class="menu" :class="{ 'open': isMenuOpen }">
      <a href="#">Sobre Mim</a>
      <a href="#services">Serviços</a>
      <a href="#portfolio">Portfólio</a>
      <a href="#contact">Contato</a>
    </nav>
  </div>
</template>

<style scoped>
header {
  text-align: center;
  background-color: rgb(180, 168, 185);
  padding: 10px;
  color: #fff;
  font-size: 24px;
  text-transform: uppercase;
  letter-spacing: 2px;
  width: 100%;
  position: fixed;
  z-index: 100;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.menu {
  background-color: #eee;
  padding: 10px;
  text-align: center;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease-in-out;
}

.menu.open {
  max-height: 500px;
}

.menu a {
  display: block;
  padding: 10px;
  color: #333;
  text-decoration: none;
  font-size: 18px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
  margin-bottom: 10px;
}

.menu a:hover {
  color: #f99;
}

.menu-toggle {
  font-size: 24px;
  color: white;
  cursor: pointer;
}

.menu {
  padding: 0;
  background-color: rgba(238, 238, 238, 0.93);
  top: 80px;
  left: 0;
  width: 100%;
  max-height: 0;
  overflow: hidden;
  position: fixed;
  transition: max-height 0.3s ease-in-out;
  z-index: 100;
}

.menu.open {
  max-height: 500px;
}

.menu-toggle {
  background-color: white;
  color: rgb(180, 168, 185);
  display: block;
  position: absolute;
  top: 20px;
  right: 20px;
}
</style>

<script setup lang="ts">
import { ref } from 'vue';

const isMenuOpen = ref(false);

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value;
}
</script>
