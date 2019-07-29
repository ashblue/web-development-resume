<template>
  <div class="ab-o-bio-card">
    <img class="ab-o-bio-card__pic" src="./../../assets/ash-blue.jpg" />
    <div class="ab-o-bio-card__info">
      <h1 class="text-center font-weight-bold display-4">Ash Blue</h1>
      <h2 class="text-center h6">Senior Web Developer</h2>
      <ListIconLinks/>
    </div>
  </div>
</template>

<script>
import ListIconLinks from '../molecules/ListIconLinks.vue';

export default {
  name: 'BioCard',
  components: {
    ListIconLinks,
  },
};
</script>

<style scoped lang="scss">
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
}
</style>
