<template>
  <div class="ab-p-home">
    <MobileBioCard class="ab-p-home__header d-lg-none" />

    <div class="container">
      <Intro></Intro>
    </div>

    <div class="footer">
      <div class="container">
        <div class="row">
          <div class="col col-lg-4">
            <p class="mb-4">
              This custom resume is hosted through GitHub pages and deployed via Travis CI
              as an open source project. <a href="#">Source code</a> available for your
              viewing pleasure.
            </p>
          </div>
        </div>
      </div>

      <p class="small text-center">
        &copy; Ash Blue, No Rights Reserved, {{currentYear}}
      </p>
    </div>
  </div>
</template>

<script>
import Intro from '../organisms/Intro.vue';
import MobileBioCard from '../organisms/MobileBioCard.vue';

export default {
  name: 'Home',
  components: {
    MobileBioCard,
    Intro,
  },
  data: () => ({
    currentYear: new Date().getFullYear(),
  }),
};
</script>

<style lang="scss">
  .ab-p-home {
    &__header {
      position: relative;
      height: 400px;
    }
  }
</style>
