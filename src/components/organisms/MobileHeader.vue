<template>
  <div class="ab-o-mobile-header">
    <div class="ab-o-mobile-header__overlay"></div>
    <img class="ab-o-mobile-header__background" src="./../../assets/ash-blue-mobile.jpg" />
  </div>
</template>

<script>
export default {
  name: 'MobileHeader',
};
</script>

<style scoped lang="scss">
  .ab-o-mobile-header {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 500px;

    &__overlay {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
      background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 1));
    }

    &__background {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
</style>
