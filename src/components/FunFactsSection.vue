<template>
  <v-sheet class="text-center pa-16" style="background-color: #298abe">
    <div class="text-h3 font-weight-bold mb-5 mb-12" style="color: #ffffff">
      Ваше задоволення – наш пріоритет!
    </div>

    <v-container>
      <v-row align="center" class="mx-15">
        <v-col v-for="item in agency" :key="item.title" cols="12" md="3" sm="6">
          <v-img height="56" :src="item.icon" />

          <div class="text-h4 font-weight-bold mt-5" style="color: #ffffff">
            {{ item.title }}
          </div>

          <div class="text-body-1 mt-5" style="color: #ffffff">
            {{ item.description }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
const agency = [
  {
    icon: 'srs/assets/agency/completed.png',
    title: '1050+',
    description: 'дзеркал, які знову радують наших клієнтів',
  },
  {
    icon: 'src/assets/agency/heart.png',
    title: '217k',
    description: 'посмішок, які ми допомогли створити',
  },
  {
    icon: 'src/assets/agency/awards.png',
    title: '1210',
    description: 'позитивних відгуків від вдячних клієнтів',
  },
  {
    icon: 'src/assets/agency/anchor.png',
    title: '2137',
    description: 'разів ми сказали "так" складним завданням',
  },
];
</script>
