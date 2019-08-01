<template>
  <div class="ab-p-home">
    <MobileBioCard class="ab-p-home__header d-lg-none" />

    <div class="ab-p-home__content overflow-hidden">
      <div class="container position-relative">
        <Intro></Intro>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
import Intro from '../organisms/intro/Intro.vue';
import MobileBioCard from '../organisms/bio-cards/FullBleedBioCard.vue';
import Footer from '../organisms/Footer.vue';

export default {
  name: 'Home',
  components: {
    MobileBioCard,
    Intro,
    Footer,
  },
  data: () => ({
    currentYear: new Date().getFullYear(),
  }),
};
</script>

<style lang="scss">
  .ab-p-home {
    display: flex;
    min-height: 100vh;
    flex-direction: column;

    &__header {
      position: relative;
      height: 400px;
    }

    &__content {
      flex: 1;
    }
  }
</style>
