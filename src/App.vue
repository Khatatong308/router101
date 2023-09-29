<script setup>
import { RouterLink, RouterView } from 'vue-router'
import BlogHeader from '@/views/BlogHeader.vue'


</script>

<template>
  <!--<RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink>-->

<div class="container">
  <br><h1 style="text-align: center; font-size: x-large;"></h1>
  <BlogHeader style="margin-top: 30px;"></BlogHeader><br>


  <div class="main">
    <RouterView />
  </div>
</div>

<div class="footer"></div>

</template>





<style scoped>

</style>
