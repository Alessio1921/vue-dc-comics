<template>
  <div id="app">
    <Header />
    <Jumbo />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbo from './components/Jumbo.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin: 0 auto;
  color: #2c3e50;
}
.my-container{
    width: 75%;
    margin: 0 auto;
}
</style>
