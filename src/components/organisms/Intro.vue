<template>
  <div>
    <div class="row mt-4 mb-5">
      <div class="col-4 d-none d-lg-block">
        <BioCard />
      </div>

      <div class="col">
        <h2 class="text-lowercase h1">
          About Me
        </h2>

        <p>
          Hi, I'm <strong>Ash Blue</strong>. A <em>senior web developer</em> with 10+
          years of experience creating web applications. My career has brought me from
          San Francisco's startup scene to fortune 500s. I specialize in JavaScript full stack with
          CI/CD to help teams create cutting edge solutions.
        </p>

        <div class="mb-5">
          <h3 class="text-hide">Details</h3>

          <div class="row">
            <div class="col-3">
              <Icon namespace="fas" icon="clock" />&nbsp;
              <span class="text-uppercase font-weight-bold small align-text-bottom">Age</span>
            </div>

            <div class="col">
              {{age}}
            </div>
          </div>

          <div class="row">
            <div class="col-3">
              <Icon namespace="fas" icon="map-marker" />
              <span class="text-uppercase font-weight-bold"> Location</span>
            </div>

            <div class="col">
              Denver
            </div>
          </div>

          <div class="row">
            <div class="col-3">
              <Icon namespace="fas" icon="phone" />
              <span class="text-uppercase font-weight-bold"> Phone</span>
            </div>

            <div class="col">
              <a href="tel:312-344-3792">312-344-3792</a>
            </div>
          </div>

          <div class="row">
            <div class="col-3">
              <Icon namespace="fas" icon="envelope" />
              <span class="text-uppercase font-weight-bold"> Email</span>
            </div>

            <div class="col">
              <a href="mailto:ash@blueashes.com">ash@blueashes.com</a>
            </div>
          </div>
        </div>

        <Resume />
      </div>
    </div>
  </div>
</template>

<script>
import BioCard from './BioCard.vue';
import Icon from '../atoms/Icon.vue';
import Resume from './Resume.vue';

function getBirthday() {
  const birthday = new Date(1987, 8, 25);
  const difference = Date.now() - birthday.getTime();
  return new Date(difference).getUTCFullYear() - 1970;
}

export default {
  name: 'Intro',
  components: {
    Resume,
    Icon,
    BioCard,
  },
  data: () => ({
    age: getBirthday(),
  }),
};
</script>

<style scoped>

</style>
