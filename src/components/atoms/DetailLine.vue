<template>
  <div class="ab-a-detail-line d-flex flex-row">
    <div class="ab-a-detail-line__title">
      <Icon class="ab-a-detail-line__icon text-center" :icon=icon :namespace=iconNamespace />&nbsp;
      <span class="text-uppercase font-weight-bold small align-text-bottom">{{title}}</span>
    </div>

    <div class="col-md col-6">
      <slot />
    </div>
  </div>
</template>

<script>
import Icon from './Icon.vue';

export default {
  name: 'DetailLine',
  components: {
    Icon,
  },
  props: {
    title: String,
    icon: String,
    iconNamespace: String,
  },
};
</script>

<style scoped lang="scss">
  @import "~bootstrap/scss/functions";
  @import "~bootstrap/scss/variables";
  @import "~bootstrap/scss/mixins/_breakpoints";

  .ab-a-detail-line {
    @include media-breakpoint-up(md) {
      &__title {
        min-width: 180px;
      }
    }

    &__icon {
      min-width: 20px;
    }
  }
</style>
