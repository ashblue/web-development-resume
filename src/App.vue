<template>
  <div class="container">
    <Intro></Intro>
  </div>
</template>

<script>
import Intro from './components/organisms/Intro.vue';

export default {
  name: 'app',
  components: {
    Intro,
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
