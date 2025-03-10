<template>
  <v-app>
    <Header />
    
    <v-main>
      <Hero />
      <SearchForm />
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

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SearchForm,
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
