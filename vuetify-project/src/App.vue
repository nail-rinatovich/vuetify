<template>
  <v-app>
    <Header />
    
    <v-main>
      <Hero />
      <SearchForm />
      <Date />
      <FeaturedApartments />
    </v-main>

    <Footer />
  </v-app>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import SearchForm from './components/SearchForm.vue'
import FeaturedApartments from './components/FeaturedApartments.vue'
import Footer from './components/Footer.vue'
import Date from './components/Date.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SearchForm,
    Date,
    FeaturedApartments,
    Footer
  }
}
</script>

<style>
.v-application {
  font-family: 'Roboto', sans-serif;
}
</style>
