<template>
  <v-sheet class="py-16">
    <v-container>
      <v-row>
        <v-col cols="12" md="5"> <v-img :src="discoverImg" /></v-col>

        <v-col cols="12" md="7">
          <div class="text-h4">
            Дізнайтеся, як ми допоможемо повернути дзеркала вашого авто до ідеального стану!
          </div>

          <div class="text-body-1 text-medium-emphasis my-5">
            Ми спеціалізуємося на професійному ремонті автодзеркал, що допомагає заощадити ваші кошти та час. Забудьте про заміну – відновимо якість швидко та ефективно!t
          </div>

          <div
            v-for="text in discover"
            :key="text"
            class="text-medium-emphasis my-2 mb-4"
          >
            <v-icon color="accent" icon="mdi-check-bold" start />

            {{ text }}
          </div>

          <v-btn
            style="background-color: #298abe; color: #ffffff"
            flat
            height="55"
            rounded
            text="Дізнатися більше"
          />
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
import discoverImg from '@/assets/discover_bg.png';
const discover = [
  'Видалення подряпин та потертостей – повертаємо дзеркалам ідеальну прозорість.',
  'Ремонт тріщин та відколів – без необхідності заміни деталей.',
  'Нанесення захисного покриття – запобігає новим пошкодженням та відблискам',
];
</script>
