<template>
  <div class="panorama-slider">
    <div class="swiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide" v-for="(image, index) in images" :key="index">
          <img class="slide-image" :src="imagePath(image.path)" alt="image" />
        </div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const images = ref([
  {path:'1.jpg', name:'nature'},
  {path:'2.jpg', name:'night-sky'},
  {path:'3.jpg', name:'chicken'},
  {path:'4.jpg', name:'moon'},
  {path:'5.jpg', name:'nature2'},
  {path:'6.jpg', name:'nature3'},
  {path:'7.jpg', name:'chameleon'},
  {path:'8.jpg', name:'car'},
  {path:'9.jpg', name:'birds'},
  {path:'10.jpg', name:'car2'},
  {path:'11.jpg', name:'car3'},
  {path:'12.jpg', name:'perfume'},
]);
function imagePath(image) {
  return new URL(`../assets/media/${image}`, import.meta.url).href;
}
</script>

<style scoped>
.panorama-slider {
  width: 100%;
  height: auto;
}
.swiper-slide img {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}
</style>
