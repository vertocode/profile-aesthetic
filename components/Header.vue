<template>
  <div>
    <header>
      Érica Esteticista
    </header>
    <nav class="menu">
      <a href="#">Sobre Mim</a>
      <a href="#services">Serviços</a>
      <a href="#portfolio">Portfólio</a>
      <a href="#contact">Contato</a>
    </nav>
  </div>
</template>

<style scoped>
header {
  background-color: rgb(180,168,185);
  padding: 20px;
  text-align: center;
  color: #fff;
  font-size: 24px;
  text-transform: uppercase;
  letter-spacing: 2px;
}
.menu {
  background-color: #eee;
  padding: 10px;
  text-align: center;
}
.menu a {
  display: inline-block;
  padding: 10px;
  color: #333;
  text-decoration: none;
  font-size: 18px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
  margin-right: 20px;
}
.menu a:hover {
  color: #f99;
}
</style>
<script setup lang="ts">
</script>
