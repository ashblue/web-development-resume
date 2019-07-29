<template>
  <ul class="list-unstyled d-flex justify-content-center">
    <!-- @TODO Feed off of a list -->
    <li class="px-1">
      <IconLink
        title="GitHub"
        icon="github"
        url="https://github.com/ashblue"
      />
    </li>
    <li class="px-1">
      <IconLink
        title="Twitter"
        icon="twitter"
        url="https://twitter.com/ashbluewd"
      />
    </li>
    <li class="px-1">
      <IconLink
        title="LinkedIn"
        icon="linkedin"
        url="https://www.linkedin.com/in/ashblue"
      />
    </li>
  </ul>
</template>

<script>
import IconLink from '../atoms/IconLink.vue';

export default {
  name: 'ListIconLinks',
  components: {
    IconLink,
  },
};
</script>

<style scoped>

</style>
