<template>
  <v-parallax
    src="https://cdn.pixabay.com/photo/2016/11/18/17/46/house-1836070_1280.jpg"
    height="600"
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col
        cols="12"
        md="8"
        class="text-center"
      >
        <h1 class="text-h2 font-weight-bold mb-4 white--text">
          Найдите идеальную квартиру для проживания
        </h1>
        <v-btn
          x-large
          color="primary"
          class="mt-4"
        >
          Поиск квартир
        </v-btn>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  name: 'Hero'
}
</script> 