<template>
  <v-sheet id="work" class="text-center py-16">
    <div class="text-h4 font-weight-bold">
      Наші роботи
    </div>

    <div class="text-body-1 text-medium-emphasis mt-5">
      Дивіться наші проекти, що виконані для наших клієнтів.
    </div>

    <v-container>
      <v-row
        class="mt-5 ga-7 pa-10"
        style="min-height: 600px"
      >
        <v-col class="d-flex flex-column align-between ga-7">
          <v-row class="h-50 bg-grey-lighten-1 rounded">
            <v-img
              src="@/assets/car_window.png"
              cover
            />
          </v-row>

          <v-row class="h-50 bg-grey-lighten-1 rounded">
            <v-img
              src="@/assets/car_window.png"
              cover
            />
          </v-row>
        </v-col>

        <v-col class="bg-grey-lighten-1 rounded" style="padding: 0">
          <v-img
              src="@/assets/car_window.png"
              cover
              class="w-100 h-100"
            />
        </v-col>

        <v-col class="d-flex flex-column align-between ga-7">
          <v-row class="h-30 bg-grey-lighten-1 rounded">
            <v-img
              src="@/assets/car_window.png"
              cover
            />
          </v-row>

          <v-row class="h-30 bg-grey-lighten-1 rounded">
            <v-img
              src="@/assets/car_window.png"
              cover
            />
          </v-row>

          <v-row class="h-30 bg-grey-lighten-1 rounded">
            <v-img
              src="@/assets/car_window.png"
              cover
            />
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>
