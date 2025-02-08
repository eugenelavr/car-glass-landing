<template>
  <v-sheet id="about" class="py-16 text-center" color="secondary">
    <div class="text-h4 font-weight-bold">Що ми робимо</div>

    <div
      class="text-body-1 font-weight-regular mt-3 text-medium-emphasis mb-12"
    >
    Дізнайтеся, як наша команда професіоналів може допомогти вам повернути дзеркала в ідеальний стан.
    </div>

    <v-container>
      <v-row>
        <v-col
          v-for="item in whatWeDo"
          :key="item.title"
          class="d-flex flex-column align-center"
          cols="12"
          md="4"
        >
          <img :src="item.icon" class="w-75 h-50" />

          <div class="text-h6 mt-1">
            {{ item.title }}
          </div>

          <div class="text-body-1 mt-2 text-medium-emphasis w-75">
            {{ item.description }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
const whatWeDo = [
  {
    icon: 'src/assets/what/scratch.png',
    title: 'Полірування та видалення подряпин',
    description:
      'Надаємо дзеркалам нового вигляду, усуваючи подряпини та потертості.',
  },
  {
    icon: 'src/assets/what/crack.png',
    title: 'Ремонт тріщин і відколів',
    description:
      'Відновлюємо пошкоджені дзеркала, щоб уникнути дорогої заміни.',
  },
  {
    icon: 'src/assets/what/antiglare.png',
    title: 'Антивідблискове покриття',
    description:
      'Захищаємо дзеркала від сонячних відблисків для комфортного водіння.',
  },
];
</script>
