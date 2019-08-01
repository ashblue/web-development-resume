<template>
  <i v-bind:class="[namespace, `fa-${icon}`]"></i>
</template>

<script>
export default {
  name: 'Icon',
  props: {
    icon: String,
    namespace: {
      type: String,
      default: 'fab',
    },
  },
};
</script>
