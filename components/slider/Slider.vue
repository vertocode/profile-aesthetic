<template>
  <main class="slider">
    <h3></h3>
    <b-carousel
      :interval="4000"
      controls
      indicators
      style="text-shadow: 1px 1px 2px #333; height: 500px;"
      background="#E9876E"
    >
      <b-carousel-slide
        v-for="image in images"
        :img-src="image.image"
      ></b-carousel-slide>
    </b-carousel>
  </main>
</template>
<script setup>

const props = defineProps({
  images: Array
})
</script>

<style>
.carousel-control-prev-icon, .carousel-control-next-icon {
  background-color: rgb(180,168,185);
  color: black;
}
.carousel-item img {
  height: 500px !important;
  max-width: 1500px;
  margin: auto;
}
</style>
