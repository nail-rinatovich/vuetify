<template>
  <v-container class="my-8">
    <v-card class="pa-4">
      <v-row>
        <v-col cols="12" md="3">
          <v-text-field
            label="Город"
            outlined
            dense
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="3">
          <v-select
            :items="rooms"
            label="Количество комнат"
            outlined
            dense
          ></v-select>
        </v-col>
        <v-col cols="12" md="3">
          <v-text-field
            label="Цена от"
            type="number"
            outlined
            dense
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="3">
          <v-btn
            color="primary"
            block
            height="40"
          >
            Найти
          </v-btn>
        </v-col>
      </v-row>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: 'SearchForm',
  data: () => ({
    rooms: ['Студия', '1', '2', '3', '4+']
  })
}
</script> 