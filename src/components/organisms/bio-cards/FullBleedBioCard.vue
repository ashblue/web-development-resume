<template>
  <div class="ab-o-mobile-bio-card">
    <img class="ab-o-mobile-bio-card__background" src="./../../../assets/ash-blue-mobile.jpg" />
    <div class="ab-o-mobile-bio-card__overlay"></div>
    <who-am-i class="ab-o-mobile-bio-card__info"></who-am-i>
  </div>
</template>

<script>
import WhoAmI from './WhoAmI.vue';

export default {
  name: 'FullBleedBioCard',
  components: {
    WhoAmI,
  },
};
</script>

<style scoped lang="scss">
  .ab-o-mobile-bio-card {
    &__overlay {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
      background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 1));
    }

    &__background {
      width: 100%;
      height: 100%;
      object-fit: cover;
      position: absolute;
    }

    &__info {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
    }
  }
</style>
