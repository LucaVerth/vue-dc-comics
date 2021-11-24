<template>
  <div id="app">
    <Header/>
    <Main/>
    <Section/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Section from './components/Section.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Section,
    Footer
  }
}
</script>

<style lang="scss">
@import  "./assets/style/Generals.scss";

</style>
