<template>
  <div class="container">
    <div id="app">
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div>

    <button class="btn btn-primary">
      <i class="fas fa-download"></i>
    </button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~@fortawesome/fontawesome-free/css/all.css";

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
