<template>
  <div id="app">
    <!-- Header -->
    <Header/>

    <!-- Products Main -->
    <main>
      <MainContent/>
        
      <MainNav/>
    </main>

    <!-- Footer -->
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainContent from './components/MainContent.vue';
import MainNav from './components/MainNav.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    MainNav,
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
