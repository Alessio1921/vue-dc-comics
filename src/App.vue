<template>
  <div id="app">
    <Header />
    <main>
      <MainContent />
    </main>

      <Footer />
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
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
