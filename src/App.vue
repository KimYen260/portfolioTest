<template>
<div id="app">
  <NavBar />
  <McBody />
  <Footer />
</div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import McBody from './components/McBody.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    NavBar,
    McBody,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
