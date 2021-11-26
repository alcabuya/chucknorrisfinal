<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Chuck1 msg="Welcome to Your Vue.js App"/>
    <Chuck2 msg="Chuck 2"/>
  </div>
</template>

<script>
import Chuck1 from './components/Chuck1.vue'
import Chuck2 from './components/Chuck2.vue'

export default {
  name: 'App',
  components: {
    Chuck1,
    Chuck2
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
  margin-top: 60px;
}
</style>
