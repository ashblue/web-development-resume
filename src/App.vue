<template>
  <Home/>
</template>

<script>
import Home from './components/pages/Home.vue';

export default {
  name: 'app',
  components: {
    Home,
  },
};
</script>

<style lang="scss">
@import "styles/colors";
@import "~bootstrap/scss/bootstrap";
@import "~@fortawesome/fontawesome-free/css/all.css";
</style>
