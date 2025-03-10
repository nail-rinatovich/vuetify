<template>
  <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="primary white--text text-center"
      width="100%"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="white--text pt-0">
        Мы поможем вам найти идеальную квартиру для проживания. Большой выбор квартир в разных районах города.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        <strong>Телефон:</strong> +7 (999) 123-45-67<br>
        <strong>Email:</strong> info@rental-apartments.ru<br>
        <strong>Адрес:</strong> ул. Примерная, д. 123, офис 45
      </v-card-text>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Аренда Квартир</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: 'Footer',
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-instagram',
      'mdi-whatsapp'
    ]
  })
}
</script> 