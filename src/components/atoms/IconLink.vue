<template>
  <a
    class="h4"
    target="_blank"
    :href="url"
    :title="title"
  >
    <Icon :icon="icon"></Icon>
    <span class="text-hide">{{title}}</span>
  </a>
</template>

<script>
import Icon from './Icon.vue';

export default {
  name: 'IconLink',
  props: {
    icon: String,
    title: String,
    url: String,
  },
  components: {
    Icon,
  },
};
</script>
