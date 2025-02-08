<template>
  <v-sheet
    id="contact"
    class="text-center py-16"
    style="background-color: #298abe; color: #ffffff;"
  >
    <div class="text-white text-h4 font-weight-medium">
      Зв'яжіться з нами
    </div>

    <div class="text-center text-body-1 mb-15">
      Якщо у вас є питання, зв'яжіться з нами сьогодні.
    </div>

    <v-container>
      <v-row>
        <v-col cols="6">
          <v-text-field
            bg-color="transparent"
            flat
            hide-details
            label="Ваше ім'я*"
            single-line
            variant="outlined"
          />
        </v-col>

        <v-col cols="6">
          <v-text-field
            bg-color="transparent"
            flat
            hide-details
            label="Ваша електронна пошта*"
            single-line
            variant="outlined"
          />
        </v-col>

        <v-col cols="6">
          <v-text-field
            bg-color="transparent"
            flat
            hide-details
            label="Номер телефону*"
            single-line
            variant="outlined"
          />
        </v-col>

        <v-col cols="6">
          <v-text-field
            bg-color="transparent"
            flat
            hide-details
            label="Вид послуги*"
            single-line
            variant="outlined"
          />
        </v-col>

        <v-col cols="12">
          <v-textarea
            bg-color="transparent"
            flat
            hide-details
            label="Ваше повідомлення..."
            lines="4"
            variant="outlined"
          />
        </v-col>
      </v-row>
    </v-container>

    <v-btn
      class="px-10 text-body-1"
      color="white"
      flat
      height="55"
      text="ЗВ'ЯЗАТИСЯ"
    />
  </v-sheet>
</template>
