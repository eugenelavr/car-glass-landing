<template>
  <v-sheet class="d-flex align-center justify-center py-16 flex-wrap ga-5 px-4">
    <v-img
      v-for="item in banners"
      :key="item"
      max-height="50"
      max-width="160"
      :src="item"
      style="background-color: #ffffff"
    />
  </v-sheet>
</template>

<script setup>
import bmw from '@/assets/banner/bmw_logo.png';
import audi from '@/assets/banner/audi_logo.png';
import vw from '@/assets/banner/vw_logo.png';
import ford from '@/assets/banner/ford_logo.png';

const banners = [bmw, audi, vw, ford];
</script>
