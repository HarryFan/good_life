<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
  
    <GoodLife />
  </div>
</template>

<script>
import GoodLife from './components/GoodLife.vue';

export default {
  name: 'App',
  components: {

    GoodLife
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
