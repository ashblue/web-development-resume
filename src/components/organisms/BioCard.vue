<template>
  <div class="ab-o-bio-card">
    <img class="ab-o-bio-card__pic" src="./../../assets/ash-blue.jpg" />
    <div class="ab-o-bio-card__gradient"></div>
    <div class="ab-o-bio-card__info">
      <h1 class="text-center font-weight-bold display-4 mb-3">Ash Blue</h1>
      <h2 class="text-center h6 mb-3">Senior Web Developer</h2>
      <ListIconLinks class="mb-4" :iconLinks="iconLinks" />
    </div>
  </div>
</template>

<script>
import ListIconLinks, { IconLinkData } from '../molecules/ListIconLinks.vue';

export default {
  name: 'BioCard',
  components: {
    ListIconLinks,
  },
  data: () => ({
    iconLinks: [
      new IconLinkData('GitHub', 'github', 'https://github.com/ashblue'),
      new IconLinkData('Twitter', 'twitter', 'https://twitter.com/ashbluewd'),
      new IconLinkData('LinkedIn', 'linkedin', 'https://www.linkedin.com/in/ashblue'),
    ],
  }),
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
