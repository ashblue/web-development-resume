<template>
  <div>
    <!-- @TODO Move this content into a page -->
    <MobileHeader class="d-lg-none" />

    <div class="container">
      <Intro></Intro>
    </div>
  </div>
</template>

<script>
import Intro from './components/organisms/Intro.vue';
import MobileHeader from './components/organisms/MobileHeader.vue';

export default {
  name: 'app',
  components: {
    MobileHeader,
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
