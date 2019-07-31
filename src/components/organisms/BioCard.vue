<template>
  <div class="ab-o-bio-card">
    <img class="ab-o-bio-card__pic" src="./../../assets/ash-blue.jpg" />
    <div class="ab-o-bio-card__gradient"></div>
    <who-am-i class="ab-o-bio-card__info mb-4"></who-am-i>
  </div>
</template>

<script>
import WhoAmI from './WhoAmI.vue';

export default {
  name: 'BioCard',
  components: {
    WhoAmI,
  },
};
</script>

<style scoped lang="scss">
@import "~bootstrap/scss/bootstrap";

.ab-o-bio-card {
  position: relative;

  &__info {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
  }

  &__pic {
    max-width: 100%;
    width: 100%;
  }

  &__gradient {
    background: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 1));
    position: absolute;
    bottom: 0;
    left: 0;
    height: 55%;
    width: 100%;
  }
}
</style>
