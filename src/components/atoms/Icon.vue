<template>
  <i v-bind:class="['fab', `fa-${icon}`]"></i>
</template>

<script>
export default {
  name: 'Icon',
  props: {
    icon: String,
  },
};
</script>

<style scoped lang="scss">
</style>
