<script setup>
  import banner from '@/assets/beef-wellington-recipe-1605882724.jpg'
  import bannerSmall from '@/assets/beef-wellington-recipe-1605882724_300.jpg'
  import bannerMedium from '@/assets/beef-wellington-recipe-1605882724_600.jpg'
  import bannerLarge from '@/assets/beef-wellington-recipe-1605882724_1000.jpg'
  import Image from '../components/Image.vue'

  const bannerSrcSet = `${bannerSmall} 320w, ${bannerMedium} 640w, ${bannerLarge} 1030w`
</script>

<template>
  <div class="banner">
    <p style="color: #FFF;">Home page view</p>
    <Image :class="'banner__img'" :alt="'Home page banner'" :src="banner" :srcset="bannerSrcSet" :sizes="'100vw'" :width="'980'" :height="'981'" />
  </div>
</template>

<style scoped>
.banner {
  position: relative;}
.banner__img {
  max-height: 300px;
}
.banner__header {
  position: absolute;
  bottom: 0;
  
}
</style>
