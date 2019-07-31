<template>
  <ul class="list-unstyled">
    <li v-for="icon in icons"
        v-bind:key="icon"
        class="fa-3x">
      <Icon :icon="icon" />
    </li>
  </ul>
</template>

<script>
import Icon from '../atoms/Icon.vue';

export default {
  name: 'ListIcons',
  components: {
    Icon,
  },
  props: {
    icons: Array,
  },
};
</script>
