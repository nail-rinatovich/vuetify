<template>
  <v-container class="my-8">
    <h2 class="text-h4 mb-6 text-center">Популярные предложения</h2>
    <v-row>
      <v-col
        v-for="apartment in apartments"
        :key="apartment.id"
        cols="12"
        sm="6"
        md="4"
      >
        <v-card>
          <v-img
            :src="apartment.image"
            height="250"
          ></v-img>
          <v-card-title>{{ apartment.title }}</v-card-title>
          <v-card-text>
            <div class="text-h6 primary--text">{{ apartment.price }} ₽/месяц</div>
            <div>{{ apartment.location }}</div>
            <div class="mt-2">{{ apartment.description }}</div>
          </v-card-text>
          <v-card-actions>
            <v-btn
              color="primary"
              text
            >
              Подробнее
            </v-btn>
            <v-btn
              color="primary"
              outlined
            >
              Забронировать
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'FeaturedApartments',
  data: () => ({
    apartments: [
      {
        id: 1,
        title: 'Современная студия',
        price: '30000',
        location: 'Центральный район',
        description: 'Уютная студия с современным ремонтом и всей необходимой мебелью',
        image: 'https://cdn.pixabay.com/photo/2016/11/18/17/46/living-room-1835923_1280.jpg'
      },
      {
        id: 2,
        title: 'Двухкомнатная квартира',
        price: '45000',
        location: 'Приморский район',
        description: 'Просторная квартира с видом на парк',
        image: 'https://cdn.pixabay.com/photo/2017/03/22/17/39/kitchen-2165756_1280.jpg'
      },
      {
        id: 3,
        title: 'Трехкомнатная квартира',
        price: '60000',
        location: 'Московский район',
        description: 'Семейная квартира в тихом районе',
        image: 'https://cdn.pixabay.com/photo/2016/11/18/17/46/house-1836070_1280.jpg'
      }
    ]
  })
}
</script> 