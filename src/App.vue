<template>
  <div id="app">
    <Header />
    <div class="container">
      <h2>都道府県</h2>
      <Prefecture />
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Prefecture from "./components/Prefecture.vue";

export default {
  name: "App",
  components: {
    Header,
    Prefecture,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.container {
  max-width: 1020px;
  margin: 0px auto;
}

h2 {
  margin-left: 5px;
}
</style>
