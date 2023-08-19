<template>
  <main class="slider">
    <h3>{{ title }}</h3>
    <b-carousel
      :interval="4000"
      controls
      indicators
      style="text-shadow: 1px 1px 2px #333; max-height: 500px; overflow: hidden;"
      background="#E9876E"
    >
      <b-carousel-slide
        v-for="(image, index) in images"
        :key="index"
        :img-src="image.image"
      ></b-carousel-slide>
    </b-carousel>
  </main>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  images: Array,
  title: String
});
</script>

<style>
.slider {
  margin: 20px auto;
  max-width: 1200px;
  overflow: hidden;
}

.carousel-control-prev-icon,
.carousel-control-next-icon {
  background-color: rgb(180, 168, 185);
  color: black;
}

.carousel-item img {
  height: 500px !important;
  max-width: 1500px;
  margin: auto;
}
</style>
