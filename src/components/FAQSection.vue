<template>
  <v-sheet
    class="text-center"
    min-height="700"
    color="secondary"
  >
    <div class="text-h4 font-weight-medium pt-15 ">
      Поширені питання
    </div>

    <v-container>
      <v-row class="pa-10 text-left">
        <v-col
          v-for="n in 4"
          :key="n"
          class="pa-10"
          cols="12"
          md="6"
        >
          <div class="text-h6 font-weight-bold text-blue-grey-darken-2">
            Які види дзеркал ви ремонтуєте?
          </div>

          <div class="text-body-1 text-medium-emphasis mt-5">
            Ми ремонтуємо всі види дзеркал, включаючи автомобільні, домашні, офісні та інші.
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
const faqs = [
  {
    question: 'Які види дзеркал ви ремонтуєте?',
    answer: 'Ми ремонтуємо всі види дзеркал, включаючи автомобільні, домашні, офісні та інші.',
  },
  {
    question: 'Які матеріали ви використовуєте для ремонту?',
    answer: 'Ми використовуємо тільки високоякісні та сертифіковані матеріали від перевірених виробників.',
  },
  {
    question: 'Як довго триває ремонт дзеркала?',
    answer: 'Час ремонту залежить від складності пошкодження, але зазвичай це займає від кількох годин до кількох днів.',
  },
  {
    question: 'Яка вартість ремонту дзеркала?',
    answer: 'Вартість ремонту залежить від виду дзеркала, складності пошкодження та використаних матеріалів.',
  },
]
</script>
