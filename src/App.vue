<template>
  <div id="app">
    <Header />
    <Prefecture />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Prefecture from './components/Prefecture.vue'

export default {
  name: 'App',
  components: {
    Header,
    Prefecture
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
}
</style>
