<template>
  <v-sheet class="text-center pa-16" color="accent">
    <div class="text-h3 font-weight-bold mb-5 mb-12">
      Fun Facts About Our Agency
    </div>

    <v-container>
      <v-row align="center" class="mx-15">
        <v-col v-for="item in agency" :key="item.title" cols="12" md="3" sm="6">
          <v-img height="56" :src="item.icon" />

          <div class="text-h4 font-weight-bold mt-5">
            {{ item.title }}
          </div>

          <div class="text-body-1 mt-5">
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
    description: 'Projects Completed',
  },
  {
    icon: 'src/assets/agency/heart.png',
    title: '217k',
    description: 'Happy Clients',
  },
  {
    icon: 'src/assets/agency/awards.png',
    title: '1210',
    description: 'Design Awards',
  },
  {
    icon: 'src/assets/agency/anchor.png',
    title: '2137',
    description: 'Line Of Codes',
  },
];
</script>
