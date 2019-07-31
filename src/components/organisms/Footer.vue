<template>
  <div class="ab-footer text-muted">
    <div class="container mt-4">

      <div class="row">
        <div class="col-12 offset-lg-4 col-lg-4">
          <p class="mb-4">
            This custom resume is hosted through GitHub pages and deployed via Travis CI
            as an open source project. <a href="#">Source code</a> available for your
            viewing pleasure.
          </p>
        </div>

        <div class="col-12 col-lg-4">
          <span class="h3 d-block mb-0 text-lowercase">Made With</span>
          <ListIcons
            class="ab-footer__icons d-flex justify-content-between mb-4"
            :icons="madeWithIcons"
          />
        </div>
      </div>

      <div class="row">
        <div class="offset-lg-4 col">
          <p class="small text-center">
            &copy; Ash Blue, No Rights Reserved, {{currentYear}}
          </p>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import ListIcons from '../molecules/ListIcons.vue';

export default {
  name: 'Footer',
  components: {
    ListIcons,
  },
  data: () => ({
    currentYear: new Date().getFullYear(),
    madeWithIcons: [
      'vuejs',
      'bootstrap',
      'sass',
      'node',
      'github',
    ],
  }),
};
</script>

<style lang="scss" scoped>
  @import "../../styles/colors";

  .ab-footer {
    background: $colorFooter;

    &__icons {
      max-width: 400px;
    }
  }
</style>
