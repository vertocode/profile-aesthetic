<template>
  <main>
    <Header />
    <AboutMe />
    <Services />
  </main>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
</script>

<style>
.title {
  background-color: #f99;
  color: white;
}
</style>
