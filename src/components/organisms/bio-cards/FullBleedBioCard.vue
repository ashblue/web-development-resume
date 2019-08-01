<template>
  <div class="ab-o-full-bleed-bio-card">
    <img
      alt="Ash Blue"
      class="ab-o-full-bleed-bio-card__portrait mx-auto mt-4 mb-4 d-block"
      src="./../../../assets/ash-blue-mobile.jpg" />
    <who-am-i class="ab-o-full-bleed-bio-card__info mb-4"></who-am-i>
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
  @import "../../../styles/colors";

  .ab-o-full-bleed-bio-card {
    background: $colorFullBleedBackground;

    &__portrait {
      $size: 220px;
      width: $size;
      height: $size;
      object-fit: cover;
      border-radius: $size;
      border: 4px solid lighten($colorFullBleedBackground, 20%);
    }
  }
</style>
