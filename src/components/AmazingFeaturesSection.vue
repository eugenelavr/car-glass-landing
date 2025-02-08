<template>
  <v-sheet id="features" class="text-center py-16">
    <div class="text-h4 font-weight-medium">Що команда <span style="color: #298abe">ProfiGlass</span> пропонує?</div>

    <div class="text-body-1 text-medium-emphasis my-5">
      Ознайомтесь з нашими дивовижними функціями, які зроблять ремонт вашого дзеркала максимально комфортним та вигідним.
    </div>

    <v-container>
      <v-row>
        <v-col
          v-for="item in features"
          :key="item.title"
          class="d-flex ga-5 pa-5 text-left"
          cols="12"
          md="4"
        >
          <div class="mt-2">
            <v-img :src="item.icon" width="40" />
          </div>

          <div>
            <div class="text-h6 font-weight-bold">
              {{ item.title }}
            </div>

            <div class="text-body-1 text-medium-emphasis mt-2">
              {{ item.description }}
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
const features = [
  {
    icon: 'src/assets/features/bell.png',
    title: 'Експрес-ремонт',
    description:
      'Ми розуміємо, як важливо для вас швидко відновити дзеркало, тому пропонуємо послугу експрес-ремонту, який займе всього кілька годин.',
  },
  {
    icon: 'src/assets/features/support.png',
    title: 'Сертифіковані матеріали',
    description:
      'Ми використовуємо тільки високоякісні матеріали від перевірених виробників, що гарантує довговічність та надійність вашого дзеркала..',
  },
  {
    icon: 'src/assets/features/user.png',
    title: 'Досвідчені майстри',
    description:
      'Наші майстри мають багаторічний досвід роботи з різними видами автомобільних дзеркал та знають всі тонкощі їх ремонту nihis.',
  },
  {
    icon: 'src/assets/features/accessibility.png',
    title: 'Гарантія на всі види робіт',
    description:
      'Ми впевнені в якості нашої роботи, тому надаємо гарантію на всі види послуг з ремонту дзеркал.',
  },
  {
    icon: 'src/assets/features/control.png',
    title: 'Виїзд майстра',
    description:
      'Для вашої зручності ми пропонуємо послугу виїзду майстра до вас додому або в офіс.',
  },
  {
    icon: 'src/assets/features/chat.png',
    title: 'Гнучка система знижок',
    description:
      'Для постійних клієнтів та при комплексному ремонті ми пропонуємо гнучку систему знижок.',
  },
];
</script>
