<template>
  <div>
    <div class="ab-o-intro__wrapper-graphic d-none d-lg-block"></div>

    <div class="row mt-4 mb-5">
      <div class="col-4 d-none d-lg-block">
        <BioCard />
      </div>

      <div class="col">
        <div class="ab-o-intro__wrapper-offset">
          <h2 class="text-lowercase h1">
            About Me
          </h2>

          <p>
            Hi, I'm <strong>Ash Blue</strong>. A <em>senior web developer</em> with 10+
            years of experience creating web applications. My career has brought me from
            San Francisco's startup scene to fortune 500s. I specialize in JavaScript full
            stack with CI/CD to help teams create cutting edge solutions.
          </p>

          <DetailsCollection class="mb-5" />

          <Resume />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BioCard from '../bio-cards/BioCard.vue';
import Resume from './Resume.vue';
import DetailsCollection from './DetailsCollection.vue';

function getBirthday() {
  const birthday = new Date(1987, 8, 25);
  const difference = Date.now() - birthday.getTime();
  return new Date(difference).getUTCFullYear() - 1970;
}

export default {
  name: 'Intro',
  components: {
    Resume,
    DetailsCollection,
    BioCard,
  },
  data: () => ({
    age: getBirthday(),
  }),
};
</script>

<style lang="scss">
  @import "../../../styles/colors";
  @import "~bootstrap/scss/functions";
  @import "~bootstrap/scss/variables";
  @import "~bootstrap/scss/mixins/_breakpoints";

  .ab-o-intro {
    $wrapperOffset: 40px;

    &__wrapper-graphic {
      position: absolute;
      background: $colorLargeScreenContainer;
      width: 100%;
      height: calc(100% - #{$wrapperOffset * 2});
      box-sizing: content-box;
      padding-right: $wrapperOffset;
      margin: $wrapperOffset 0 0 ($wrapperOffset * -1);
    }

    @include media-breakpoint-up(lg) {
      &__wrapper-offset {
        margin: ($wrapperOffset + 20px) 0;
      }
    }
  }
</style>
