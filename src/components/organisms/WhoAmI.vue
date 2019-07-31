<template>
  <div>
    <h1 class="text-center font-weight-bold display-4 mb-3">Ash Blue</h1>
    <h2 class="text-center h6 mb-3">Senior Web Developer</h2>
    <ListIconLinks :iconLinks="iconLinks" />
  </div>
</template>

<script>
import ListIconLinks, { IconLinkData } from '../molecules/ListIconLinks.vue';

export default {
  name: 'WhoAmI',
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
