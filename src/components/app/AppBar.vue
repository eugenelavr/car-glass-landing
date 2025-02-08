<template>
  <v-app-bar>
    <template #title>
      <div
        class="d-inline-flex align-center text-h4 font-weight-bold my-5 text-primary"
      >
        <v-img :src="logo" width="200" />
      </div>
    </template>

    <template v-if="$vuetify.display.mdAndUp" #append>
      <div class="hidden-sm-and-down">
        <v-btn
          v-for="item in menu"
          :key="item.link"
          class="text-body-1 blue-grey-darken-4"
          :href="item.link"
          variant="text"
        >
          {{ item.title }}
        </v-btn>
      </div>
    </template>
  </v-app-bar>
</template>

<script setup>
import logo from '@/assets/logo/logo.png';

const menu = [
  {
    title: 'Головна',
    link: '#home',
  },
  {
    title: 'Про нас',
    link: '#about',
  },
  {
    title: 'Відгуки',
    link: '#testimonials',
  },
  {
    title: 'Роботи',
    link: '#work',
  },
  {
    title: 'Команда',
    link: '#team',
  },
  {
    title: 'Сервіс',
    link: '#features',
  },
  {
    title: 'Контакти',
    link: '#contact',
  },
];
</script>

<style>
body .v-toolbar__content > .v-toolbar-title {
  margin-inline-start: 0;
}
</style>
