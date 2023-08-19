<template>
  <main>
    <Header />
    <AboutMe />
    <Services />
    <Portfolio />
    <Contact style="margin-top: 2em"/>
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
  background-color: rgb(180,168,185);
  color: white;
}
</style>
