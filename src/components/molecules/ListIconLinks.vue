<template>
  <ul class="list-unstyled d-flex justify-content-center">
    <li v-for="iconLink in iconLinks"
        v-bind:key="iconLink.title"
        class="px-2">
      <IconLink
        :title="iconLink.title"
        :icon="iconLink.icon"
        :url="iconLink.url"
      />
    </li>
  </ul>
</template>

<script>
import IconLink from '../atoms/IconLink.vue';

export class IconLinkData {
  constructor(title, icon, url) {
    this.title = title;
    this.icon = icon;
    this.url = url;
  }
}

export default {
  name: 'ListIconLinks',
  components: {
    IconLink,
  },
  props: {
    iconLinks: Array,
  },
};
</script>

<style scoped>

</style>
