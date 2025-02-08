<template>
  <v-sheet
    id="team"
    class="text-center py-16"
    color="secondary"
    min-height="800"
  >
    <div class="text-h4 font-weight-bold">Команда <span style="color: #298abe">ProfiGlass</span></div>

    <div class="text-body-1 text-medium-emphasis mt-5">
      Дізнайтеся більше про нашу високопрофесійну команду.
    </div>

    <v-container>
      <v-row>
        <v-col
          v-for="person in team"
          :key="person.name"
          class="pa-5"
          cols="12"
          md="4"
        >
          <v-card class="bg-white rounded-t-xl pb-5" flat>
            <v-img class="w-100 rounded-t-xl" :src="person.image" />

            <div class="mt-3 text-body-1">
              {{ person.name }}
            </div>

            <div class="mt-3 text-grey-lighten-1 font-italic text-body-1">
              {{ person.title }}
            </div>

            <div class="mt-5 text-medium-emphasis mx-5">
              {{ person.description }}
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
import PersonImg from '../assets/team/person1.png'

const team = [
  {
    image: `${PersonImg}`,
    name: 'Анатолій',
    title: 'Механік',
    description:
      'Майстер по ремонту дзеркал. Досвід у сфері 10 років.',
  },
  {
    image: `${PersonImg}`,
    name: 'Анатолій',
    title: 'Механік',
    description:
      'Майстер по ремонту дзеркал. Досвід у сфері 10 років.',
  },
  {
    image: `${PersonImg}`,
    name: 'Анатолій',
    title: 'Механік',
    description:
      'Майстер по ремонту дзеркал. Досвід у сфері 10 років.',
  },
];
</script>
