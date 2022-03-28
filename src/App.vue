<template>
  <div id="app">
    <!-- Header -->
    <Header/>

    <!-- Products Main -->
    <main>
        <Products/>
    </main>

    <!-- Footer -->
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Products from './components/Products.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Products,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
