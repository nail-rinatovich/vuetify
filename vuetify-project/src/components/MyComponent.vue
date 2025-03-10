<template>
    <v-card>
      <v-card-title>Пример компонента</v-card-title>
      <v-card-text>
        <v-btn color="primary" @click="handleClick">Нажми меня</v-btn>
      </v-card-text>
    </v-card>
  </template>
  
  <script>
  export default {
    name: 'MyComponent',
    methods: {
      handleClick() {
        alert('Кнопка нажата!');
      }
    }
  }
  </script>
  
  <style scoped>
  /* Ваши стили */
  </style>